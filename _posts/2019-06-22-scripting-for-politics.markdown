---
layout: post
title: Scripting for Politics
public: true
author: giacomo
---

As promised to the members of the [Partito Pirata](https://forum.partito-pirata.it/t/registrazione-assemblea-tnt-per-il-partito-pirata-9-giugno-2019-torino-polo-culturale-lombroso16/2702/14)
(the Italian Pirate Party) I wrote a little shell script that automatically
installs a simple self-contained [PeerTube](https://joinpeertube.org/) instance
on a clean-state [Debian GNU/Linux](https://www.debian.org/).

Together with the [Project Winston Smith](https://pws.winstonsmith.org) that promised to provide hardware and bandwidth,
this little work should help all the members of the Partito Pirata to 
[avoid YouTube](https://forum.partito-pirata.it/t/possiamo-evitare-di-supportare-e-diffondere-la-sorveglianza/2465)
and to stop sending to Google's servers the political interests of the people who visit their forum and website.

In an age where programmers have [so much power](http://www.tesio.it/2019/06/03/what-is-informatics.html)
to summon daemons that act on the physical world, I think we should always feel responsible for those who
don't have access to our knowledge.

My hope with the Partito Pirata is that [they will accept the challenge](https://forum.partito-pirata.it/t/il-partito-pirata-dal-2020/2661) 
to spread [Hacker's Curiosity](https://forum.partito-pirata.it/t/chi-sono-i-pirati-sullidentita-di-questo-partito/2423/) through Informatics.

**Informatics should not be a weapon** to gain Power!  
It should be a rock to build Democracy upon.

Enough words. Here is the code:

```
#!/bin/sh

# Copyright (C) 2019 Giacomo Tesio <giacomo@tesio.it>
#
# This software is a hack and it is released accordingly under the
# Hacking License available at http://www.tesio.it/documents/HACK.txt

DOMAIN=$1
EMAIL=$2
PASSWORD=$3
TWITTER=$4

if [ "$PASSWORD" = "" ]; then

	echo usage: sudo ./peertube-install.sh domain email password twitter
	echo
	echo This script install PeerTube on a Debian GNU/Linux 9.9
	echo
	echo "  domain   is the domain name user will use to access your instance, thus"
	echo "           - A and AAAA records must be configured on your DNS"
	echo "           - it won't be easy to modify it after the installation"
	echo
	echo "  email    is the email address that will be used by Let's Encrypt"
	echo
	echo "  password is the peertube user's password on both the OS and the DB"	
	echo "           it is ALSO the instance's administrator's password"
	echo
	echo "  twitter  is a Twitter account name to be used WITH the initial @"
	echo
	echo
	echo At the end of the installation you should double-check:
	echo
	echo /var/www/peertube/config/production.yaml
	echo /etc/nginx/sites-available/peertube
	echo /etc/systemd/system/peertube.service
	echo /etc/letsencrypt/live/
	
	exit 1
fi

echo PeerTube Installation
echo

dnsError() {
	echo ERROR: cannot resolve $DOMAIN
	echo Please configure your A/AAAA record on the DNS
	exit 2
}

debinst() {
	for pkg in "$@"; do
		dpkg -l "$pkg"|grep ii > /dev/null || apt-get install -y "$pkg"
	done
}

installCertbot() {
	BACKPORT_LIST=/etc/apt/sources.list.d/backports.list
	if [ ! -f $BACKPORT_LIST ]; then
		echo -n Adding backports.list... 
		echo deb http://deb.debian.org/debian stretch-backports main > $BACKPORT_LIST
		echo done.
	fi

	apt-get update

	apt-get install -y -t stretch-backports certbot python-certbot-nginx
}

installNodeJS() {
	curl -sL https://deb.nodesource.com/setup_8.x | bash -
	debinst nodejs
}

installYarn(){
	curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
	echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list
	apt-get update && apt-get install yarn
}

initPeertubeDB() {
	sudo -u postgres psql -c "CREATE USER peertube WITH PASSWORD '$PASSWORD';"
	sudo -u postgres createdb -O peertube peertube_prod
	sudo -u postgres psql -c "CREATE EXTENSION pg_trgm;" peertube_prod
	sudo -u postgres psql -c "CREATE EXTENSION unaccent;" peertube_prod
}

createPeertubeUser() {
	if [ ! -d /var/www/peertube ]; then
		useradd -m -d /var/www/peertube -s /bin/bash -p peertube peertube
		echo "peertube:$PASSWORD"|chpasswd
		initPeertubeDB
	fi
}

installPeertube() {
	VERSION=$(curl -s https://api.github.com/repos/chocobozzz/peertube/releases/latest | grep tag_name | cut -d '"' -f 4) && echo "Latest Peertube version is $VERSION"
	cd /var/www/peertube && sudo -u peertube mkdir config storage versions && cd versions
	sudo -u peertube wget -q "https://github.com/Chocobozzz/PeerTube/releases/download/${VERSION}/peertube-${VERSION}.zip"
	sudo -u peertube unzip peertube-${VERSION}.zip && sudo -u peertube rm peertube-${VERSION}.zip
	cd ../ && sudo -u peertube ln -s versions/peertube-${VERSION} ./peertube-latest
	cd ./peertube-latest && sudo -H -u peertube yarn install --production --pure-lockfile
}

configurePeertube() {
	cd /var/www/peertube && sudo -u peertube cp peertube-latest/config/production.yaml.example config/production.yaml
	sudo -u peertube sed -i -e "s/\@Chocobozzz/$TWITTER/" config/production.yaml
	sudo -u peertube sed -i -e "s/admin\@example.com/$EMAIL/" config/production.yaml
	sudo -u peertube sed -i -e "s/example.com/$DOMAIN/" config/production.yaml
	sudo -u peertube sed -i -e "s/password: 'peertube'/password: '$PASSWORD'/" config/production.yaml	
	
	cp /var/www/peertube/peertube-latest/support/nginx/peertube /etc/nginx/sites-available/peertube
	sed -i -e "s/peertube.example.com/$DOMAIN/" /etc/nginx/sites-available/peertube
	ln -s /etc/nginx/sites-available/peertube /etc/nginx/sites-enabled/peertube
	
	# configure let's encrypt
	systemctl stop nginx
	sed -i -e "s/ssl_certificate/#ssl_certificate/" /etc/nginx/sites-available/peertube # Comment ssl_certificate and ssl_certificate_key lines
	certbot --authenticator standalone --installer nginx --post-hook "systemctl start nginx" -n --agree-tos -m "$EMAIL" --domains "$DOMAIN"
	sed -i -e "s/#ssl_certificate/ssl_certificate/" /etc/nginx/sites-available/peertube # Uncomment ssl_certificate and ssl_certificate_key lines
	systemctl reload nginx
}

tuneTCPIP() {
	cp /var/www/peertube/peertube-latest/support/sysctl.d/30-peertube-tcp.conf /etc/sysctl.d/
	sysctl -p /etc/sysctl.d/30-peertube-tcp.conf
}

setupSystemd(){
	cp /var/www/peertube/peertube-latest/support/systemd/peertube.service /etc/systemd/system/
	systemctl daemon-reload
	systemctl enable peertube
	systemctl start peertube
	journalctl -feu peertube
}

# check domain resolution (or Let's Encrypt will complain)
getent hosts $DOMAIN  > /dev/null || dnsError

# Install dependencies
debinst unzip curl

dpkg -l certbot|grep ii > /dev/null || installCertbot
dpkg -l nodejs|grep ii > /dev/null || installNodeJS
dpkg -l yarn|grep ii > /dev/null || installYarn

debinst nginx ffmpeg postgresql postgresql-contrib openssl g++ make redis-server git python-dev

systemctl start redis postgresql

# Install Peertube
export PT_INITIAL_ROOT_PASSWORD=$PASSWORD
createPeertubeUser
test -d /var/www/peertube/versions || installPeertube
test -f /etc/nginx/sites-available/peertube || configurePeertube

# TCP/IP tuning
test -f /etc/sysctl.d/30-peertube-tcp.conf || tuneTCPIP

# Systemd setup
test -f /etc/systemd/system/peertube.service || setupSystemd

```
