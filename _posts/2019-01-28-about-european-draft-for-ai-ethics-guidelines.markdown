---
layout: post
title: About European Draft for AI Ethics Guidelines
public: true
author: giacomo
---

What follows are the comments I've sent to the High-Level Expert Group
working to define AI Ethics Guidelines for the European Commission.

To understand them, you need a decent understanding of
Artificial Intelligence and Machine Learning and to read the
[DRAFT ETHICS GUIDELINES FOR TRUSTWORTHY AI](https://ec.europa.eu/futurium/en/system/files/ged/ai_hleg_draft_ethics_guidelines_18_december.pdf)

# Introduction: Rationale and Foresight of the Guidelines

The first lines of the introduction highlight a serious flaw of the draft:
the pillars that underpin the Commission’s vision show a fundamental bias:

1. increasing public and private investments in AI to boost its uptake,
2. preparing for socio-economic changes, and 
3. ensuring an appropriate ethical and legal framework to strengthen
   European values

Being eager to adopt a largely misunderstood technology obviously inhibits
the ability to reason about its limits and risks.

Before trying to boost its uptake, the Commission should try to
understand to what extent and in which fields of endeavour the set of
techniques that goes under the AI umbrella should be experimented.

As Shoshana Zuboff recently wrote, technology is NOT an unstoppable force
of nature, but a human artifact serving interests and needs of specific
humans. In other words, Technology is a prosecution of Politics by other
means: each advancement can be designed to serve the public interest or
private and elitarian ones. And just like with Politics, a renounce to
participate to its course just means to being subject to others' will.

Before talking about "Trustworthy AI", we should have a population able
to understand the topic enough for their trust to be meaningful.

As for today, without a serious investments in schools to foster
History and Informatics as preconditions of our citizenship, such trust
can not be meaningful but just deceptive and ill founded.

It's not a trust on the technology, but in the corporations and the
"experts" that can exploit such trust and the widespread ignorance of the
topic to weaken regulations and streghten their handle on society.


Having said that, the high level description outlined for the Ethical
framework is basically sound: it's reasonable to think that when the whole
population will be able to understand how a neural network's calibration
differs from a k-mean clustering, a similar framework will emerge.

However the glossary that preceed the Introduction already shows that
we are not ready for such framework: despite being written by an high
level expert group on AI, the definitions still use an antropomorphic
language to describe what is just software.
In particular describing software bugs (either intentional or
unintentional) as "bias" shows a deep misunderstanding about the software
in question and about the statistical processes that define its behaviour.
Later on, similar concerns emerge when the draft cites "non-determinism"
while talking about software that is executed by deterministic machines
(aka computers).

Such language is worrying because it shows a tendency from the HLEG to
rationalize the risks as inevitable instead of understanding them deeply 
and taking them into account.

# Chapter I: Respecting Fundamental Rights, Principles and Values - Ethical Purpose 

Despite an interesting and convidisible introduction, the principles that
the chapter proposes lack a fundamental hierarchical structure.

It should be quite evident by looking at such principles:

- The Principle of Beneficence: "Do Good"
- The Principle of Non maleficence: "Do no Harm"
- The Principle of Autonomy: "Preserve Human Agency"
- The Principle of Justice: "Be Fair"
- The Principle of Explicability: "Operate transparently"

Even if we hadn't more than two thousands years from the Hippocratic Oath
and generations of physicians grown with the "Primum non nocere" maxim, we
can see how the last three principles are just specializations of the more
general "Do no Harm". In particular the Principle of Autonomy tries to 
address risks to individuals, the Principle of Justice tries to address the
risks to weak groups and the Principle of Explicability tries to address
socio-political risks.

Since the Principle of Non Maleficience is so preponderant to require three
specializations, we should put it first, before the principle of
Beneficience, and underlining its relation with the others:

- The Principle of Non maleficence: "Do no Harm"
  - The Principle of Autonomy: "Preserve Human Agency"
  - The Principle of Justice: "Be Fair"
  - The Principle of Explicability: "Operate transparently"
- The Principle of Beneficence: "Do Good"

The road to hell is paved with good intentions: just like with medicine,
whenever simpler and safer solutions exist they should be preferred to
more complex and risky ones.



But there is an even more important omission in the list:
the Principle of Ultimate Human Accountability.

This is a fundamental principle that underlie all European ethical and legal
system: at least a human must always be accountable for the problems caused
by a human artifact.

In other terms: what is forbidden to a human can not be allowed through
an artificial proxy, no matter how "autonomous" (aka expensive to debug)
such proxy is.

Talking about ethics is void if we are not ready to enforce this simple
but fundamental principle of human responsibility.



The section on "Lethal Autonomous Weapon Systems"
is in direct contrast to all the principles stated above.

The only way an Ethical Framework can be credible while proposing
principles like "Do no Harm", "Preserve Human Agency", "Be Fair",
"Operate transparently" and "Do Good" is to clearly state that
Autonomous Weapon Systems (lethal or not) must be forbidden on the
European territory.

The section on the "Potential longer-term concerns" shows the usual sci-fi
based fears that are the flip side of the current hype.

Instead of being concerned about Artificial Consciousness that would be
way easier to fake than to implement we should be afraid of semi-autonomous
weapons in the hands of a small group of people holding most of
the planet's wealth. And in the count of such weapons we should obviously
include every tool that can be used to direct human attention, to 
manipulate feelings or perceptions and to forge mass opinions.


# Chapter II: Realising Trustworthy AI

Even this chapter present several issues:

1. The short paragraph about "Accountability" suggest to design mechanisms
   that can range from monetary compensation to apology, but it forgets to 
   include prison: to gain trust it is important to explicitly state that
   an autonomous proxy cannot become a "Get Out of Jail Free" ticket.
2. The section on "Safety" looks like it was designed to be ineffective:
   it's pointless to assess potential risks associated with the use of
   AI-based products and services without defining serious punishments when
   things goes wrong anyway.
3. The section on "Trasparency" is too vague and forgiving: a simpler
   approach is to say that no opacity must be allowed in applications that
   consume human data. Such rules would instantly skyrocket private and
   public investments in AI research, looking for new machine learning
   techniques that can be fully explained and debugged.
4. The section on "Robustness" looks well designed but open to a wide
   de-responsibilization when it improperly talks about "non-determinism"
   (false, if we are talking about deterministic, non-quantum, computers)
   and it cites "complexity", "opacity", and "sensitivity to training/model
   building conditions" as a sort of justifications for unreproducible
   results.
   Simply, whenever such conditions exists, the AI program is not robust
   and should not be applied to problems that require such robustness.
5. The section about "Human Autonomy" is very scary: in no way
   people should be nudged by machines. If AI will be successful in
   enhancing human wealth as it's  promise to be, a lot of friendly people
   with a lot of free time will be able to nudge us on our request, but
   it's too dangerous to let flawed machines manipulate humans whatever the
   goal: every software has bugs vulnerabilities and many have intentional
   backdoors: AI won't be different.

Later, in "Architectures for Trustworthy AI", while considering the
technical means to ensure an ethical behaviour the HLEG suggest to
integrate an ethical signal in the "sense" phase of the stochastic system.

This is both naive and weird:

- WHICH ethics we should use?  
  If we widely deploy autonomous machines
  following a certain ethical model, people will adapt to it (because
  machines cannot really adapt to us): this could turn to be most effective
  brain washing project ever conceived.
  Humans naturally adapt to the sorrounding intelligences: put a consumist
  agent in every room, and you will build a population of consumists.
- HOW MUCH ethics?  
  Who will decide the weight of that signal?
  And what when a bug will inhibit it?
  Or what if other inputs overwhelm such signal?
  The only use of an ethical signal in an autonomous system is to shield
  corporations from taking full responsibility of errors: it's dumb to
  pretend to teach ethics to trolleys, we should build infrastructures
  that simply prevent lethal incidents to occur.

Moreover in the section about Regulation we lack any reference to penal
justice: just like before, it should be clearly stated that when an
autonomous artifact kill or harm, one or more humans will be held fully 
accountable for it. 


# Chapter III: Assessing Trustworthy AI

I really appreciated the flexible approach to the assessment process:
talking about ethics, a checklist would be too easy to exploit.

For sure, each technique requires different kind of assessments: for
example the dataset used to calibrate a k-mean could be enough to reproduce
the calibration process and to exclude any racial discriminations, but it
would be totally inadequate for assess any property of a classifier based
on an artificial neural network.

The risk however is that, without a widespread understanding of the AI
techniques, the Commission will ask to the wolfs how to rule the sheeps:
we cannot rely on experts that consults large corporations to define
any assessment of "trust" into something that can manipulate people.

Moreover, being able to assess the Ethics of a "Trustworthy AI" cannot
replace clear regulation establishing the characteristics that an algorithm
must have before being fed with human data.

In particular we need to extend the right to "meaningful information about
the logic involved" by each AI processing beyond the individuals protected
by the article 13 of the GDPR: even groups, such as families, neightbors,
customers and so on should have the right to know and understand the exact
logic applied to their collective data, when and to which aim the
processing occurs.


# General Comments

Despite all the issues described here, I appreciated the effort and care
that has been evidently put by the HLEG in the writing of this draft.

It's important for Europe to fill our technological gap with U.S.A. and 
China and it's conforting to see serious people working on the ethical
issues that will emerge from the AI adoption.

However is even more important to avoid short-cuts.
Good will and honesty are fundamental, but not enough to balance lobbying
and hype.

To address our technological issues (including AI adoption) we need to
raise the general population understanding of Informatics. We need a new
mass education plan, with serious investments on teachers and professors
from the primary school on. We need to raise a generation of people able
to modify the software that they use and they feed with their own data.

Since Technology is Politics, being able to self-host and customize the
applications we use is the only way to preserve democracy: it will prevent
data capitalization and people manipulation.

Programming is today what Writing was during Ancient Egypt: a tool which
is totally primitive, but effective to collect and retain Power among
humans exactly because it is primitive.

We need better systems, better programming languages and people able to
use software without being manipulated through it.

Until then, widespread adoption of AI can be useful, but it's irresponsible
to apply it to human data. We need prudent regulations that err on the side
of caution, not because computer-aided statistics is dangerous in itself
but because it's too easy to abuse it and manipulate or hurt people and
societies in a context when most people can't understand their working.

