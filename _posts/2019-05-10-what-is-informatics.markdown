---
layout: post
title: What is Informatics?
public: false
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
coined the term « *Informatik* » for his essay *Informatik: Automatische 
Informationsverarbeitung*, "Informatics: automatic information processing".

On March 1962, [Philippe Dreyfus](https://en.wikipedia.org/wiki/Philippe_Dreyfus)
used for the first time the term « *Informatique* » to name his own company
*Société d'informatique appliquée*.

On the same month Walter Bauer started the american company «Informatics Inc.»,
registered its trademark and sued universities using such word to
describe the new field, forcing them to resort to the locution "Computer
Science", despite the fact that the matter was not restricted to computers
and the [scientific method](https://en.wikipedia.org/wiki/Scientific_method)
was not really applied by practicioners.

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
is full of interesting dichotomy. The most fundamental but often overlooked
one is that between Information and Data:

> **Information**, from Latin *informo*, "I build in my mind":
> An idea, a construct of a human mind that can be shared with other humans.
>
> **Datum**, pl. **Data**, from Latin *datum*, "given":
> One of the possibile representations of a piece of information that can be
> transferred and interpreted as information by humans.

Information only exists in a human mind.

Not every construct of a human mind is information, but only
those that can be precisely comunicated to other humans.
For example, no [mystic experience](https://en.wikipedia.org/wiki/Mysticism)
can be really shared.

However Information is the fundamental building block of human
[knowledge](https://en.wikipedia.org/wiki/Knowledge).
For example, whatever belongs to the 
[field of Mathematics](http://www.tesio.it/2018/10/11/math-science-and-technology.html)
is Information, so much that no conjecture can be considered as a valid statement
until other humans can agree on it just by reading the
[description of the proof](https://mathbabe.org/2012/08/06/what-is-a-proof/)
that was formed in the author's mind.

Data instead are mere representations.

Any representation of Information is actually a datum.

The words you are reading, be them printed on paper or drawn on a raster
screen, just represent a message I'm trying to convey, an insight built
over years of practice in the field.

But I could have recorded a video lesson, for example.

Or recorded a [phonograph](https://en.wikipedia.org/wiki/Phonograph_record).

All of these would have been representation of the same information.
But they would not be equivalent.

## A complex relationship

Information and data have a very complex relation.

By writing these words I'm turning the information to data.  
By reading them, you are turning the data back to information again.

Both of above sentences are properly expressed in present tense, but they
occur at different points in time.

Moreover data always convey much more information than the intended one.
For example the information about this text itself, its language, its
length and so on, are what is often improperly called
"[metadata](https://en.wikipedia.org/wiki/Metadata)".
But even a lot of personal information is embedded in these data,
as the style of my writings might reveal.

If instead of a text the message was carried through a video
a whole lot of other informations would be spread together with the
intended message.

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

It's about humans not machines. Computers are mere mirrors for our own minds.

As it often happens, this European perspective is diametrically opposed to
the American one [attributed to Knuth](https://fr.wikipedia.org/wiki/Informatique#%C3%89tymologie).

Yet in [a well known essay](http://www.maa.org/programs/maa-awards/writing-awards/computer-science-and-its-relation-to-mathematics), 
Knuth defines Computer Science as "the study of Algorithms"
while they are so unrelated to computers that he can also use a game of
"musical chairs" to describe the inner working of [hash tables](https://en.wikipedia.org/wiki/Hash_table)
in that same paper.

The problem of naming is not "just" a philsophical one: after
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
just because humans are inheritely fallible.

Each program is just one of the many possible representations of an
algorithm and, together with the algorithm itself, it also conveys 
[a whole lot of other informations](https://www.usenix.org/system/files/conference/usenixsecurity15/sec15-paper-caliskan-islam.pdf).

Moreover, if the programmer does not know the **full** algorithm he is
trying to implement beforehand, bugs become just another example of the
more general principle known as "[Garbage In, Garbage Out](https://en.wikipedia.org/wiki/GIGO)".

Bugs are so inheritely tied to the real world of Informatics that
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
excluding [cryptography](https://en.wikipedia.org/wiki/Side-channel_attack),
[Statistics](https://en.wikipedia.org/wiki/Machine_learning),
[UX design](https://en.wikipedia.org/wiki/Human%E2%80%93computer_interaction) and so on.

And while this statement might look heretic at first, it shouldn't surprise
us much as we can see that Informatics is changing every single field of 
human endeavours, from Medicine to Agriculture, from Reproduction to Finance,
from Engineering to Cooking, from Democracy to War.

And while no program need Medicine, most Doctors use programs.  
And while no program need to kill, most War need software.  
And so on.

This weird phenomenon also has a simple explaination: Informatics changes
everything humans do because **it changes how humans collectively think**.
Indeed, if Information belongs to a human mind, when shared among the
members of community, it builds the Culture of such community. And such
Culture goes back into new members' minds as Information in a never
ending feedback loop.

Informatics is today what Mathematics was at the time of [Pythagoras](https://en.wikipedia.org/wiki/Pythagoras).  
It's Philosophy on disguise. Applied Philosophy, if you will.

# A Political field

Many practicioners would refuse this qualification of Informatics
as a modern form of Philosophy. It's not just because of ignorance
about Philosophy itself (that is where Logic, was born). 
It's because of a bad feeling about it.
After all, if you look at the history, from Confucius to Plato,
from Kant to Nietzsche, **philosophers have always had this 
weird habit of messing with Politics** one way or another.

This is annoying. Software Engineers pretends to be Engineers so
that they can focus their minds on technical stuffs **alone**.
They feel responsible to create the best possible artifact
that can serve a purpose, but don't want to accountable for
the choice of the purpose itself.

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

In itself, a general purpose computer is useless.
But programs can specialize them to make them useful for a wide variety of problems.


As before, each progress in the technology of weapons provided a
strategic advantage to those who got it. We don't need to go back at the
stone age to see evidence of this. Not even knowing about Enigma is required.
A Cyber World War is ongoing right now. A war for the total domination
of humans through technology.


## The value of Debugging

There is nothing on Earth that can train [Critical Thinking](https://en.wikipedia.org/wiki/Critical_thinking)
as a decade or two of [Software Debugging](https://en.wikipedia.org/wiki/Debugging).

Programming in itself is useful to learn how to describe complex dynamic
and ever evolving systems to somebody as **dumb** as a computer is.
Some [techniques](https://en.wikipedia.org/wiki/Domain-driven_design) are
so similar to Philosophy that practicioners talk way more than they code.

The programming language you use also influence your way of thinking in a
way that is way deeper than what you eperience when learning a human language.
The patterns you learn while programming becomes useful in every aspect of
your own life. Exactly like with Math, but on steroids.


And yet, the real key to understand the political potential of Informatics is
**debugging**. While debugging **you look for an error in the collective
cultural elaboration of thousands of people** from all over the world.

You see a computer executing billions of lines of code and you have to
guess where somebody did the error that is currently causing a
misbehaviour. It's such an expensive and complex task, that people and
corporations try to avoid it as much as possible, usually working around
the bug. But if you **have** to fix it, it's a very **educative** experience.

First because most of times, it's your own fault.

But sometimes it's really the compiler. Sometimes it's really the operating system.
Sometime it's really the browser's garbage collector.
Sometimes you see the [butterfly effect](https://en.wikipedia.org/wiki/Butterfly_effect)
happening: you **have** to find (and kill) the right butterfly hundreds of
miles away, just to stop the tornado you are in. 

Compared to this, **debunking a Fake News is a kids game**.

Compared to this, debunking lobbists' claims is a kids game!

That's because you are trained to get an insight about what
thousands of other people have thought before you, to grasp
their assumptions, to spot not only what they knew or what
they misunderstood but what they didn't knew at all.

The Unknown is a first class citizen of Informatics.

Good programmers [know that they know nothing](https://en.wikipedia.org/wiki/Socratic_method). By experience.  
And hackers know that **nobody knows anything**. That's why we are so curious!


# A Universal Human Right

In the Universal Declaration of Human Rights, three articles talk about
Informatics without even knowing about it:

12)
No one shall be subjected to arbitrary interference with his privacy,
family, home or correspondence, nor to attacks upon his honour and reputation.
Everyone has the right to the protection of the law against such interference
or attacks.

19)
Everyone has the right to freedom of opinion and expression; this right
includes freedom to hold opinions without interference and to seek, receive
and impart information and ideas through any media and regardless of frontiers.

27)
(1) Everyone has the right freely to participate in the cultural life of
    the community, to enjoy the arts and to share in scientific advancement
    and its benefits.
(2) Everyone has the right to the protection of the moral and material
    interests resulting from any scientific, literary or artistic
    production of which he is the author.

Even without looking at the large multinational corporations that
constitute the core of Surveillance Capitalism, we can see that these
articles are sistematically violated from most computer device that we "own".

People who cannot configure their own mail server, cannot have 12 granted.
People who cannot program themselves, cannot "impart information and ideas
through any media" and thus cannot have 19 granted.
People who cannot debug a cryptographic library, cannot have 19 granted
Since programs are culture (and theorems, by Curry–Howard correspondence),
people who cannod program cannot have 27.1 granted.


As complex artifacts build on top of the work of several people. software
are always collective works. They are culture.
