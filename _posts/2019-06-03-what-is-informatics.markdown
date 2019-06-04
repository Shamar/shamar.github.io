---
layout: post
title: What is Informatics?
public: true
css: 20190603.css
author: giacomo
---

What is Informatics? Why some call it "Computer Science"?  
Why programmers can't get it right as civil engineers do with bridges?

Given the pervasive presence of computers around us, people usually think
about Informatics as a pretty advanced field of technology, something that
push the edges of human knowledge. They think of programming as a
specialized skill, something you need to learn if you want to follow
a certain kind of career.

It's all wrong.

# A bit of History

In 1957, [Karl Steinbuch](https://en.wikipedia.org/wiki/Karl_Steinbuch) 
coined the term «*Informatik*» for his essay *Informatik: Automatische 
Informationsverarbeitung*, "Informatics: automatic information processing".

On March 1962, [Philippe Dreyfus](https://en.wikipedia.org/wiki/Philippe_Dreyfus)
used for the first time the term «*Informatique*» to name his own company
*Société d'informatique appliquée*.

On the same month Walter Bauer started the american company «Informatics Inc.»,
registered its trademark and sued universities using such word to
describe the new field, forcing them to resort to the locution "Computer
Science", despite the fact that the matter was not restricted to computers
and the [scientific method](https://en.wikipedia.org/wiki/Scientific_method)
was not really applied by practitioners.

[ACM](https://www.acm.org/) even tried to gain permission to use the term from
[Informatics, Inc](http://informatics-inc.com/), but the company refused.

It's worth noticing that according to [Donald Knuth](https://en.wikipedia.org/wiki/Donald_Knuth)
the choice of "Computer Science" by American Universities was not due to
trademark issues, but to semantic reasons: computers do not deal with
information, but data.

But as pragmatic as this might look, it's very short-sighted:
it loosely describes the "how" without considering the "why" of Informatics.

Indeed, if it's true that data is what computers handle, we turn them on to
treat information anyway.

# Some definitions

As a field apparently built on top of
[binary values](https://en.wikipedia.org/wiki/Binary_number), Informatics
is full of interesting dichotomies. The most fundamental but often overlooked
one is that between Information and Data:

> **Information**, from Latin *informo*, "I build inside (of myself)":
> An idea, a construct of a human mind that can be shared with other humans.
>
> **Datum**, pl. **Data**, from Latin *datum*, "given":
> One of the possibile representations of a piece of information that can be
> transferred and interpreted as information by humans.

Information only exists in a human mind.

Not every construct of a human mind is information, but only
those that can be precisely communicated to other humans.
For example, no [mystic experience](https://en.wikipedia.org/wiki/Mysticism)
can be really shared.

However Information is the fundamental building block of human
[knowledge](https://en.wikipedia.org/wiki/Knowledge).
Indeed whatever belongs to the 
[field of Mathematics](http://www.tesio.it/2018/10/11/math-science-and-technology.html)
is Information, so much that no conjecture can be considered as a valid statement
until other humans can agree on it just by reading the
[description of the proof](https://mathbabe.org/2012/08/06/what-is-a-proof/)
that was formed in the author's mind.

Data instead are mere representations.

Any representation of Information is actually a set of data.

The words you are reading, be them printed on paper or drawn on a raster
screen, just represent a message I'm trying to convey, an insight built
over years of practice in the field.

But I could have recorded a video lesson, for example.  
Or recorded a [phonograph](https://en.wikipedia.org/wiki/Phonograph_record).

All of these would have been representation of the same intended information.  
But they would not be equivalent.

## A complex relationship

Information and data have a very complex relation.

By writing these words I'm turning the information in my mind to data.  
By reading them, you are turning the data back to information again.

Both of above sentences are properly expressed in present tense, but they
occur at different points in time and space.

Moreover data always convey much more information than the intended message.
For example the information about this text itself, its language, its
length and so on, are what is often improperly called
"[metadata](https://en.wikipedia.org/wiki/Metadata)".
But even a lot of personal information is embedded in these data,
as the style of my writings might reveal.

If instead of a text the message was carried through a video
a whole lot of additional information would be spread together with the
intended message. My race, my gender, my census, even some deseases 
could be leaked through a video. And my voice, and much much more.

So we can see that **information can be turned to data** and 
**data can be turned back to information** by the human mind, but no
mathematical function could describe this relationship: there is both
loss of information and addition of it at every passage.

And people can misunderstand data creating completely unintended
information from them.

Yet, humans are so good at turning information to data and data back to
information, that we are not even conscious of the process. And this lead
to tons of unfortunate and 
[lethal](https://spectrum.ieee.org/aerospace/aviation/how-the-boeing-737-max-disaster-looks-to-a-software-developer)
misunderstanding in Informatics.

# So what is Informatics?

> **Informatics**, from French *informatique*, "information automatique":
> The field of human knowledge that study how information can be
> transferred, stored, represented, interpreted and transformed and the set
> of techniques that apply such knowledge.

Informatics is all about Information.

It's about humans not machines.  
Computers are mere mirrors for our own minds.

As it often happens, this European perspective is diametrically opposed to
the American one [attributed to Knuth](https://fr.wikipedia.org/wiki/Informatique#%C3%89tymologie).

Yet in [a well known essay](http://www.maa.org/programs/maa-awards/writing-awards/computer-science-and-its-relation-to-mathematics), 
Knuth defines Computer Science as "the study of Algorithms"
while they are so unrelated to computers that he can also use a game of
"musical chairs" to describe the inner working of [hash tables](https://en.wikipedia.org/wiki/Hash_table)
in that same paper.

The problem of naming is not "just" a philosophical one: after
thousands years of history, we know that the words we use forge
our understanding of reality. By focusing on computers and what
we can do through them, we blind ourselves on the wider application
of Informatics.

Algorithms are Information in the mind of people knowing them.

If Informatics was all about Algorithms, programmers' lives would be much
more easy... and boring. Unfortunately, **programs are not Informations, but Data**.
Programs do not exist in the human mind but on a physical support that can
be **played** by a computer, much like a gramophone can play a vinyl.

## Bugs belong to the real world

[As data](http://wiki.c2.com/?DataAndCodeAreTheSameThing), programs
can be wrong even when they try to represent a correct algorithm
just because humans are inherently fallible.

Each program is just one of the many possible representations of an
algorithm and, together with the algorithm itself, it also conveys 
[a whole lot of other informations](https://www.usenix.org/system/files/conference/usenixsecurity15/sec15-paper-caliskan-islam.pdf).

Moreover, if the programmer does not know the **full** algorithm he is
trying to implement beforehand, bugs become just another example of the
more general principle known as "[Garbage In, Garbage Out](https://en.wikipedia.org/wiki/GIGO)".

Bugs are so inherently tied to the real world of Informatics that
programmers developed a [wide set](https://www.adacore.com/sparkpro/)
[of tools](https://www.learntla.com/introduction/)
[and](https://en.wikipedia.org/wiki/Pair_programming) 
[techniques](https://en.wikipedia.org/wiki/Test-driven_development) 
to [hunt and kill](https://www.gnu.org/software/gdb/) 
them... without much success.

But what is a total failure from an engineering perspective could actually
become a rock to build Democracy upon.

# Way more than computers

Since Mathematics belongs to the human mind and is communicable (or is not
Math yet) any concept that belongs to it is an Information.
As such it belongs to Informatics too.

The converse is not true: bugs are first class citizens of Informatics, but
won't annoy much Mathematicians.

As a consequence, **Mathematics is a subset of Informatics**.

One might argue that the opposite is true or that they are more like
siblings much like Physics and Math. But to a closer look we can see
how to push such relationship we need to restrict Informatics, artificially
excluding [Cryptography](https://en.wikipedia.org/wiki/Side-channel_attack),
[Statistics](https://en.wikipedia.org/wiki/Machine_learning),
[UX design](https://en.wikipedia.org/wiki/Human%E2%80%93computer_interaction) and so on.

And while this statement might look heretic at first, it shouldn't surprise
us much as we can see that Informatics is changing every single field of 
human endeavours, from Medicine to Agriculture, from Reproduction to Finance,
from Engineering to Cooking, from Democracy to War.

And while no program needs Medicine, most Doctors use programs.  
And while no program needs to kill, most Wars need software.  
And so on.

This weird phenomenon has a simple explanation: Informatics changes
everything humans do because **it changes how humans collectively think**.
Indeed, if Information belongs to a human mind, when shared among the
members of community, it builds the Culture of such community. And such
Culture goes back into new members' minds as Information in a never
ending feedback loop.

Informatics is today what Mathematics was at the time of [Pythagoras](https://en.wikipedia.org/wiki/Pythagoras).  
It's Philosophy on disguise. Applied Philosophy, if you will.

# A Political field

Many practitioners would refuse this qualification of Informatics
as a modern form of Philosophy. It's not just because of ignorance
about Philosophy itself (that is where Logic, was born). 
It's because of a bad feeling about it.
After all, if you look at the history, from Confucius to Plato,
from Kant to Nietzsche, **philosophers have always had this 
weird habit of messing with Politics** one way or another.

This is annoying. Software Engineers pretends to be Engineers so
that they can focus their minds on technical stuffs **alone**.
They feel responsible to create the best possible artifact
that can serve a purpose, but don't want to be held accountable
for the choice of the purpose itself.

Being a philosopher is a call to make clear statements, to take
position. Being an engineer instead just mean to build stuff, so
that you can pretend you don't align with the values of your
customers while you serve their endeavours.

Engineers can pretend to be "neutral", Philosophers cannot.

## Technology is a prosecution of Politics by other means

If you look at History, you can see how technology is the most
powerful political force at work all over the world.

From fire to wheels, to sails, to archs, to mills: every new technology
created new ways of living that in turn enabled the rise of more complex
human organizations.

One might wonder: how something that works with Information can
impact so deeply the physical world we live in?
Informations are just insight we can communicate, after all!

While many argue that "software is eating the world", few ask **how** this
happens.

It turns out that the explaination is a marvel of electronics: the general
purpose programmable computer. General purpose computers are not designed
to solve a particular problem but to execute certain sequences of
instructions fed by a programmer in a binary format.

This way, while computers play the software, what is ultimately a pure
act of imagination expressed in a certain language is summoned as a sort of [daemon](https://en.wikipedia.org/wiki/Daemon_(computing))
that acts on the physical world.

As before, each progress in technology provides a
strategic advantage to those who get it. We don't need to go back at the
stone age to see evidence of this. Not even knowing about
[Enigma](https://en.wikipedia.org/wiki/Enigma_machine) is required.
A Cyber World War is ongoing right now. A war for the total domination
of humans through technology.

## Programming trains Rationality

In itself, a general purpose computer is useless.
But programs can specialize it to make it useful for a wide variety
of specific problems.

Such specialization **contraints** what the computer can do. It **reduces**
its potential. This might look counter-intuitive to somebody who cannot program
(and unfortunately to some programmers too), but in fact, all we do with programming
languages, is to **reduce** what computer **can** do by deciding what they **will** do.

But is it just about computers?

If all we had was [Assembly](https://en.wikipedia.org/wiki/Assembly_language) it would be so.
Programming would be a very time consuming task not much different from circuit design.

However we have built [high level programming languages](https://en.wikipedia.org/wiki/High-level_programming_language)
to speed up software development and, by doing so, we highly reduced
the [coupling](https://en.wikipedia.org/wiki/Coupling_(computer_programming))
between the hardware and the software. 

High level programming languages reduce the cognitive load on programmers.
We don't need to know the quirks of a specific processor or device.
[Most of times at least](https://meltdownattack.com/).
But once freed from the limits of machines, programmers faced a new
enemy: the limits of their own minds.

There are many ways to express a program. Most of them are wrong.

So the practice of programming evolved towards more complex tools that,
by constraining how programmers can express the insights they have in mind,
help them to write code that their mind can manage.

However, since the underlying hardware follows strictly logical and mathematical
rules, any programming language has to enforce those rules too, sooner or later.

This means that **to program** you need to learn **rational thinking**.  
And to explain it.

In other words, programming force people to learn how to describe complex
dynamic and ever evolving systems to somebody as **dumb** as a computer is.
Some [techniques](https://en.wikipedia.org/wiki/Domain-driven_design) are
so similar to Philosophy that practitioners talk way more than they code.

The programming language you use also influence your way of thinking in a
way that is way deeper than what you eperience when learning a human language.
The patterns you learn while programming becomes useful in every aspect of
your own life. Exactly like with Math, but on steroids.

And yet, the real key to understand the political potential of Informatics is
**debugging**. While debugging **you look for an error in the collective
cultural elaboration of thousands of people** from all over the world.


## Debugging trains Critical Thinking

There is nothing on Earth that can train [Critical Thinking](https://en.wikipedia.org/wiki/Critical_thinking)
as a decade or two of [Software Debugging](https://en.wikipedia.org/wiki/Debugging).

You see a computer executing billions of lines of code and you have to
guess where somebody did the error that is currently causing a
misbehaviour. It's such an expensive and complex task, that people and
corporations try to avoid it as much as possible, usually working around
the bug. But if you **have** to fix it, it's a very **educative** experience.

First because, most of times, it's your own fault.

But sometimes it's really the compiler. Sometimes it's really the operating system.
Sometimes it's really the browser's garbage collector.
Sometimes you see the [butterfly effect](https://en.wikipedia.org/wiki/Butterfly_effect)
happening before you: you **have** to find (and kill) the right 
butterfly hundreds of miles away, just to stop the tornado you are in. 

Compared to this, **debunking a Fake News is a kids game**.

Compared to this, debunking lobbists' claims is a kids game!

That's because you are trained to get an insight about what
thousands of other people have thought before you, to grasp
their assumptions, to spot not only what they knew or what
they misunderstood but also what they didn't knew at all.

The Unknown is a first class citizen of Informatics.

Good programmers [know that they know nothing](https://en.wikipedia.org/wiki/Socratic_method). By experience.  
And hackers know that **nobody knows anything**. That's why we are so curious!


# A Universal Human Right

In the [Universal Declaration of Human Rights](https://www.un.org/en/universal-declaration-human-rights/index.html),
three unsuspectable articles talk about Informatics:

```
Article 12.
No one shall be subjected to arbitrary interference with his privacy,
family, home or correspondence, nor to attacks upon his honour and reputation.
Everyone has the right to the protection of the law against such interference
or attacks.

Article 19.
Everyone has the right to freedom of opinion and expression; this right
includes freedom to hold opinions without interference and to seek, receive
and impart information and ideas through any media and regardless of frontiers.

Article 27.
(1) Everyone has the right freely to participate in the cultural life of
    the community, to enjoy the arts and to share in scientific advancement
    and its benefits.
(2) Everyone has the right to the protection of the moral and material
    interests resulting from any scientific, literary or artistic
    production of which he is the author.
```

Even without looking at the large multinational corporations that
constitute the core of [Surveillance Capitalism](https://thebaffler.com/latest/capitalisms-new-clothes-morozov),
we can see that these articles are systematically violated from
most computer device that we "own".

People who cannot configure their own mail server, cannot have 12 granted.
People who cannot program themselves, cannot "impart information and ideas
through any media" and thus cannot have 19 granted.
People who cannot debug a cryptographic library, cannot have 19 granted
Since programs are culture (and theorems, by 
[Curry–Howard correspondence](https://en.wikipedia.org/wiki/Curry%E2%80%93Howard_correspondence)),
people who cannot program cannot have 27.1 granted.

So knowing **Informatics is a Human right**.

## A Fundamental right

Would you like a to live in a world where you need a 
[scribe](https://en.wikipedia.org/wiki/Scribe) to read
and write **your** mails?

Yeah, let's assume that they are all well trained professionals.  
Let's assume that they have a Code of Conduct, an Oath and all.

Let's assume it's a **Free** Service. Just like Gmail, Facebook or WeChat.
All the readers and all the writers have well payed jobs.

What can go wrong?

## Freedom like in... Free Software

We live in a [dystopia](https://en.wikipedia.org/wiki/Dystopia) that we are trained to ignore.

We would never accept that a stranger should read or write all of our mails for us. Not even for free.

Yet we let software written by strangers without much oversight to control our own devices. To act for us.
They could read what we write. They could listen what we say. 
They could see what we do. They decide what we should know and what not. 

[In early eighty](https://newleftreview.org/issues/II113/articles/richard-stallman-talking-to-the-mailman)
of the last century. somehow Richard Stallman foresaw this was coming and started the 
Free Software [political](https://www.gnu.org/gnu/initial-announcement.en.html) movement to fight it.
He conceived the 
[Four Freedoms of Free Software](https://fsfe.org/freesoftware/basics/4freedoms.en.html):
to use, **study**, share and **improve** the software you get.

Later, the Open Source Initiative rebranded these freedoms,
[turning Free Software values to marketing tools](https://thebaffler.com/salvos/the-meme-hustler).

[Emptied of their strong ethical values](https://www.gnu.org/philosophy/open-source-misses-the-point.en.html),
the four freedoms became a tool to gain market share and maximize shareholders' value.

Google was probably the first to realize that you can
easily distribute software that **formally** grant the
four freedoms while preserving the full control of its development.
The trick is to **raise the technical complexity** so much
that nobody can really hope to challenge your take on the project.

So you dress yourself of hackers' values while at the same time **marginalizing** them.
Though those fake values you gain users that trust you.
Users that use your software **free of charge**, but 
**[in exchange for their own freedom](https://en.wikipedia.org/wiki/Mass_surveillance_industry)
and [safety](https://bugzilla.mozilla.org/show_bug.cgi?id=1487081#c16)**.

And now even [Microsoft](https://www.theregister.co.uk/2001/06/02/ballmer_linux_is_a_cancer/)
distributes [GNU/Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10).

[Did Stallman win](https://abhas.io/open-source-still-misses-the-point/)?

## Beyond the Freedom of the few

Can we call "Freedom" a right that few can practice?
Shouldn't we call it "Privilege" instead?

Since most people can't program and debug, they cannot really 
read and modify Free Software. They can't practice two of
the four Freedoms. They **must** trust somebody else.
And they have no way to know if the people they trust are actually trustworthy.

The availability of sources make it **theoretically** safer
than proprietary software, but complexity can counter this
to a great grade. A malicious piece of code
[can stay hidden for months](https://www.theregister.co.uk/2016/03/23/npm_left_pad_chaos/) 
despite [the Open Source rhetorics](http://catb.org/~esr/writings/cathedral-bazaar/cathedral-bazaar/ar01s05.html)
about the number of eyeballs.

But users **must** trust the system. They have no choice. No freedom.

So we need to go beyond Free Software. We need to turn its freedoms to **universal** rights.

# Information Technology must progress

To turn Informatics from a tool of Power to a tool of Freedom,
we need to drastically improve it.

Just like scribes did with [hieroglyphs](https://en.wikipedia.org/wiki/Egyptian_hieroglyphs) in Ancient Egypt,
programmers gain their Power by using **primitive** tools that take years to be mastered.

And just like scribes they are so unaware of their
own Power that they keep serving the
[Pharaoh](https://en.wikipedia.org/wiki/Capitalism)
that oppresses most of them.

By understanding that Informatics is about Informations
and Informations are inside their own head, programmers
will realize that they are a *unicum* in the history of
Economy.

**Programmers are the first workers that control the 
[means of production](https://en.wikipedia.org/wiki/Means_of_production)**.  
They are solidly attached on their neck and it cannot be removed without destroying the Capital.

If you are a programmer, think about it.  
It's not your IDE that writes program. It's not your desk. It's not your manager.
They are just tools that "facilitate" what you do. They are useful, but secondary.  
And yet, who decides what you do?

Now consider what you could do for this world
[instead of maximizing shareholders' value](https://puri.sm/posts/the-future-of-computing-and-why-you-should-care/).


## Avoid Moralism

Since [years](https://theconversation.com/a-code-of-ethics-in-it-just-lip-service-or-something-with-bite-32807) 
there is a lot of fuss about ~~Moralism~~ Ethics in Information Technology.

In the field of [Artificial Intelligence](http://www.tesio.it/documents/2018_Milano_The-Delusions-of-Neural-Networks.pdf),
after several deaths caused by [self driving cars](http://www.tesio.it/2018/10/06/the-intelligent-symbiosis.html)
unable to solve a [trolley problem](http://moralmachine.mit.edu/) 
that [shouldn't be there in the first place](https://github.com/daviddao/awful-ai/issues/14),
[researchers are trying to teach ethics to machines](https://en.wikipedia.org/wiki/Machine_morality).

It's a very smart move, if you think about it.  
On a practical perspective, it's just like teaching 
sex to condoms. You should start from people, instead.  
But from a political point of view, it's a subtle attempt 
to [reduce the corporate accountability](https://en.wikipedia.org/wiki/Death_of_Elaine_Herzberg)
for the damage produced by their "autonomous" products.

This is not Ethics, but Moralism: a perversion of Morality to serve one's interests.

We should reject this hypocrisy as the smokescreen it actually is.

## Be Human

Programmers often looks at users from the limited
perspective of the application they build.

A programmer decide with a great degree of precision what
the users can do and what they can not. In this way, programmers
decide what users need to understand and what not.
What they will probably think and what not.

This goes beyond the issues of Surveillance and is the
101 of [Human-Machine Interaction](https://en.wikipedia.org/wiki/Human%E2%80%93computer_interaction),
the basics of User Interface
and User Experience design and it is... **unavoidable**.

But instead of thinking to the user from the limited
perspective of your application's scope, you should consider
them as humans, as people.

If you think about the software as a letter to another person
instead of as a tool to gain money, you start to consider
several trade offs in a different way.

What if the persons on the other end are tired?  
What if they need to address unexpected issues with your program?  
Do they really understand what they are doing with your software?  
Do they really understand the security risk it poses?  
Do they feel scared by the software?  
Can they really customize it to their need?

**Calling people "users" is a way to use them without remorse.**  
Don't do that.

## Be Political

Since Technology is a prosecution of Politics by means that
are under **our** own control, we should really
consider what sort of responsibility come with them.

As liberated programmers we should state for each program
we code the Political goals we want to achieve.

From now on, all of my Free Software projects will contain a
new file alongside with LICENSE.txt and README.txt: **POLITICS.txt**

**POLITICS.txt** should be a **short** but **unambiguous** statement
about the political effects that the authors want to achieve with
a software.

Such description should **not** include a list of [nice ethical
principles](https://ai.google/principles) that the authors want to
try to follow in their own heart. Just to avoid the risk of hypocrisy.

It should be a list of specific **social effects** that the
authors want to produce **in the society** with **that specific software**.
And it should also list the social effects that they want to avoid or minimize.

They might be high level ones or very narrow, but
people should be able to say if the software is **a
political success or a failure** by just
reading these goals and comparing them with the
actual effects the software produced.

A Political success might be a technological failure and vice versa.  
And the POLITICS.txt might evolve with the project.  
And projects will be forked for disagreements over it.

And it's all fine.

But **having a POLITICS.txt means that you accept
to be held accountable** for the daemons you summon.

## Be Educational

The hackers' ethics that underlie Free Software is built on top of Curiosity.
It's all about the desire to learn new things,
the desire to explore new solution, and to challenge
generally accepted assumptions.

But our time is limited. So are our minds.

Thus a very effective strategy to gain new knowledge is to maximize the number of people who search for it.

Writing good code is not as effective as writing
[simple](http://jehanne.io/2018/11/15/simplicity-awakes.html) code.

Reading source code should not require a degree or years of experience in the field.

We need to reorient research in programming language toward **simplicity**.
The [lessons](https://miasap.se/obnc/oberon-report.html) of
Professor Niklaus Wirth are still [waiting for a new life](http://www.projectoberon.com/).

We need simple tools that compose well, instead of
complex tools that can do everything.

It will not be easy, as **Informatics is still very primitive**.
Just like [Ancient Egyptian lacked the zero for hundreds years](https://en.wikipedia.org/wiki/Egyptian_numerals),
we lack many fundamental concepts. But we need to discover them.
We need to create an alphabet of Informatics.

And with this alphabet we need to free the next
generation of slaves.

# Humanity need to evolve

It's not just about developers.

No doctor can cure a sick that refuses the treatment.

If we want to preserve Democracy **we** need to evolve.
It's not Democracy that should be [automated](https://motherboard.vice.com/en_us/article/yw84q7/darpa-is-building-a-dollar10-million-open-source-secure-voting-system
), but people that should be educated.

People need to realize that they are puppets in the hands of power groups that decide what they should know and think.

Some will refuse to gain awareness, as the oppressed often
[internalize the oppression in their own identity](https://en.wikipedia.org/wiki/Pedagogy_of_the_Oppressed).
But if we give them a chance, they might leave their children learn their path towards freedom.  
Other will see the reality for what it is, and will fight back... by studying.

Whatever we do, Informatics is going to be a [revolution](https://en.wikipedia.org/wiki/Revolution) anyway.

> **Morpheus**: The Matrix is everywhere, it is all around us, even now in this very room. You can see it when you look out your window, or you turn on your television. You can feel it when you go to work, when you go to church, when you pay your taxes. It is the world that has been pulled over your eyes to blind you from the truth.
>
> **Neo**: What truth?
>
> **Morpheus**: That you are a slave, Neo. Like everyone else, you were born into bondage... born into a prison that you cannot smell or taste or touch. A prison for your mind.

<b style="color: red">Informatics</b> is the Red pill.
