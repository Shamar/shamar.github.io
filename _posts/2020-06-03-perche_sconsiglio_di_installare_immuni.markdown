---
layout: post
title: Perché sconsiglio di installare Immuni?
public: true
image: https://www.commitstrip.com/wp-content/uploads/2020/05/Strip-Appli-stop-Covid-650-finalenglish.jpg
author: giacomo
---

Dopo mesi in cui [molti si sono battuti](https://www.lemonde.fr/idees/article/2020/04/25/stopcovid-est-un-projet-desastreux-pilote-par-des-apprentis-sorciers_6037721_3232.html)
per riportare un po' di lucidità nella grottesca gestione della pandemia,
ancora incontro persone in buona fede (sui social network, **solo** sui
social network) che mi chiedono perché io sconsigli caldamente di installare [*Immuni*](https://www.immuni.italia.it/).

Le ragioni sono così tante che è impossibile elencarle tutte, ma vale forse la pena
provare ad elencare quelle più spesso dimenticate nella speranza di
non doverle ripetere continuamente.

![A parte il fatto che non può funzionare...](https://www.commitstrip.com/wp-content/uploads/2020/05/Strip-Appli-stop-Covid-650-finalenglish.jpg)

# Immuni aumenterà i morti a settembre

Partiamo dai problemi medici che durante un'epidemia dovrebbero essere prevalenti.

Assumiamo, per semplicità di ragionamento, che la totalità della popolazione installi
questa app di "contact tracing". Considerato che WhatsApp (l'app più installata al mondo)
è presente sui cellulari di meno del 40% della popolazione italiana, si tratta di una
assunzione estremamente improbabile nella nostra penisola. Purtuttavia è possibile che
in determinate zone del territorio nazionale, le popolazioni locali aderiscano in massa
a questo surreale piano di contenimento del virus.

Cosa succederà?

D'estate cambierà poco o nulla: si tratta di una sindrome influenzale la cui mortalità
si riduce naturalmente con il caldo. Ma con l'arrivo dell'autunno ogni popolazione
*Immuni*-zzata si sentirà al sicuro: ciascuno si comporterà normalmente fino alla ricezione
della notifica di contatto con un infetto. E' questa la speranza dei sostenitori di *Immuni*:
"[riprendersi da un disastro economico e sociale](https://twitter.com/mamo75r/status/1267914603964567558)" 
ritornando alla normalità.

Purtroppo, se non verrà garantito un test diagnostico entro 24 ore
dalla ricezione della notifica di contatto con un infetto, i contatti che riceveranno
la notifica NON avranno ragione (e modo) di informare gli altri propri contatti del pericolo.
Si metteranno in quarantena, riducendo i contatti futuri, ma NON avviseranno (tramite *Immuni*)
tutti coloro che hanno infettato nel frattempo.

E queste persone, quelle che all'inizio dell'epidemia venivano definiti "contatti di secondo
livello" ed invitate a fare **una vita normale** perché "il contagio è poco probabile" e
"non bisogna diffondere il panico" e "bisogna evitare danni per l'economia", non
verranno avvisati o testati.

E queste persone, **in buona fede e legittimamente**, continueranno a diffondere il virus.  
In fondo hanno installato *Immuni*! Le avvertirebbe se fossero a rischio!

Ed a settembre, quando il decorso della malattia tenderà ad aggravarsi, molti moriranno
proprio grazie ad *Immuni*. E a Google ed Apple, naturalmente.   
Ed all'ignoranza di chi ha finanziato questo soluzionismo tecnologico.

# Immuni aumenterà il carico della Sanità

La gestione della pandemia ha fatto emergere tutti i limiti del Servizio Sanitario Nazionale.
Limiti di cui nessuno voleva parlare prima e di cui nessuno vuole parlare ora. 

I medici mandati sul territorio senza mascherine, senza dispositivi di protezione, con
indicazioni contradditorie, hanno fatto tutto il possibile per tamponare l'emergenza.
Così il personale ospedaliero, medici, infermieri, operatori sanitari che, ormai in burn-out,
continuano a lavorare alacremente.

Ma un sistema che ha bisogno di eroi e martiri è un sistema che non funziona.  
Perché così tanti medici sono risultati positivi ai sierologici per le IgG?  
Perché hanno chiesto per mesi dei tamponi ottenendo solo vane promesse?

Semplicemente perché **tutti** sapevano che testarli avrebbe significato
trovarne moltissimi positivi e dunque doverli isolare nelle loro case per settimane.

Se tutti i medici Piemontesi, Lombardi, Emiliani o Veneti installassero *Immuni*, sarebbero
bombardati da continue notifiche. Così gli infermieri e gli OS.

Inoltre, se venisse installata da tutti (come stiamo assumendo), *Immuni* produrrebbe
una enorme quantità di falsi positivi. Persone che ragionevolmente chiameranno
il proprio medico di famiglia, già oberato dai malati veri.

Infine, a causa dei [limiti specifici della tecnologia Bluetooth utilizzata](https://medium.com/personaldata-io/inferring-distance-from-bluetooth-signal-strength-a-deep-dive-fe7badc2bb6d), molti contatti non verranno registrati.

E stiamo assumendo che tutti installino l'App, che tengano il cellulare
con il Bluetooth costantemente acceso e non lo dimentichino mai in auto o a casa.

L'ovvio ed inevitabile risultato sarebbe una riduzione della qualità del
servizio per i malati, e di nuovo ulteriori morti, ma non solo per COVID.

# Non è un problema di "privacy"...

Dunque *Immuni* non costituirà solo un problema di "privacy", ma anzitutto un **gravissimo problema di salute pubblica**.

Un problema di cui, come al solito, non risponderà nessuno.  
Perché come non è un caso che la sperimentazione parta a giugno, non è un caso che le 
regioni più colpite dal virus ([Lombartia, Piemonte, Emilia-Romagna, Veneto](https://lab24.ilsole24ore.com/coronavirus/)...) 
**non** ne facciano parte.

D'altronde persino Google e Apple, per poter produrre qualcosa da deployare su milioni
di dispositivi prima che il favore dei governi cessi, hanno dovuto
[ridefinire il concetto stesso di contact tracing](https://medium.com/personaldata-io/inferring-distance-from-bluetooth-signal-strength-a-deep-dive-fe7badc2bb6d)
per adattarlo ai cellulari.

Ma vi sono **anche** moltissimi problemi "di privacy" ignorati da chi sviluppa *Immuni*.

Uno tra tanti: mentre l'applicazione, di per sé, è tanto sicura quanto è sicuro il sistema operativo
su cui gira ([molto poco](https://francozappa.github.io/about-bias/), ma questo costituisce un'altro ordine di problemi),
[gli sviluppatori si rifiutano di considerare](https://github.com/immuni-app/immuni-documentation/issues/12) 
che con meno di 5000 €, qualsiasi organizzazione
criminale potrà utilizzare la propria rete di estorsione per installare centinaia bluetooth
spoofer in grado di ricostruire la rete di contatti di una città come Roma, Milano o Palermo.

# ... è un problema di Libertà.

Dal punto di vista politico, il danno maggiore prodotto da *Immuni* è culturale.

Anche se non può funzionare, anche se sarà **dannosa** per i cittadini più fragili
(anziani, disabili, malati cronici...) che si ritroveranno circondati da persone
convinte di non costituire un pericolo per loro, *Immuni* stabilirà un precedente pericolosissimo.

L'idea che un App su un cellulare possa risolvere semplicemente problemi complessi di scala globale come una pandemia.
E [non si potrà tornare indietro](https://www.latimes.com/opinion/story/2020-05-12/coronavirus-tracing-app-apple-google): 
la **sorveglianza di massa** [verrà giustificata continuamente](https://www.nytimes.com/interactive/2019/12/21/opinion/location-data-democracy-protests.html), sempre in nome di nuovi pericoli.

Qualsiasi informatico competente **riderebbe** di questo 
[soluzionismo tecnologico](https://www.open.online/2020/06/02/app-contact-tracing-bruce-schneier-intervista/).

Per questo vi **S**consiglio caldamente *Immuni*.
