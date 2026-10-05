---
id: 007
title: "Anosognosia"
subtitle: "What Alzheimer's, a stroke ward and an 1847 maternity hospital have to do with Bitcoin self-custody."
language: en
author: Yuri da Silva Villas Boas
papers: [DS]
reading_time: ~9 min
cover: assets/cover-1200x675.webp
cover_alt: "The Who Killed Hannibal meme. In the top panel a man has just shot another, who lies slumped over a sofa labeled BITCOIN STATISTICS; the shooter is labeled with the standard advice: don't tell anyone you own BTC, deny if asked, rehearse your denial, use secret tricks. In the lower panel the same man stands over the body asking why stats don't help elucidate the wrench attack crisis. The panel beside it reads Anosognosia, not knowing that you don't know, and states that this is not a measurement: it is the first of the Denial Spiral's four censoring mechanisms, a structural claim rather than a counted one, because a practice that works by not being visible leaves no record of working or of failing."
---

# Anosognosia

<p align="center"><img src="assets/cover-1200x675.webp" alt="The Who Killed Hannibal meme. In the top panel a man has just shot another, who lies slumped over a sofa labeled BITCOIN STATISTICS; the shooter is labeled with the standard advice: don't tell anyone you own BTC, deny if asked, rehearse your denial, use secret tricks. In the lower panel the same man stands over the body asking why stats don't help elucidate the wrench attack crisis. The panel beside it reads Anosognosia, not knowing that you don't know, and states that this is not a measurement: it is the first of the Denial Spiral's four censoring mechanisms, a structural claim rather than a counted one, because a practice that works by not being visible leaves no record of working or of failing." width="680"></p>

There's a word in neurology for a patient who is ill and can't tell. Joseph
Babinski coined it in 1914 for people paralyzed down one side after a stroke
who, asked to lift the paralyzed arm, would explain calmly that they didn't
feel like it, or that they just had. *Anosognosia*: not knowing that you don't
know. It turns up in Alzheimer's too, and there it's crueller, because the
disease erodes memory and, with it, the ability to notice that memory is
going. One cause, two effects, and the second hides the first.

I think Bitcoin self-custody has its own anosognosia, and I think it's the
reason nothing in this series is likely to change anything on its own.

The disease is obscurity: security that depends on the attacker not knowing
something. Decoy wallets, duress PINs, a hidden passphrase, "just don't tell
anyone you hold." The earlier posts argued that this fails, that it fails under
[Kerckhoffs](https://zenodo.org/doi/10.5281/zenodo.22778480) by construction, and that
when it fails it can turn a robbery into a
[torture](https://github.com/Yuri-SVB/great-wall-posts/tree/main/posts/004-they-only-took-my-pokemon-cards)
or a [killing](https://github.com/Yuri-SVB/great-wall-posts/tree/main/posts/006-the-deadly-race).
This one is about the anosognosia: why the field can't see it failing. There are four reasons,
and the fourth is the one that matters.

## One: obscurity does not advertise itself

For obvious reasons, obscurity would typically not advertise itself.

That's the whole of it, and I'd like to leave it there, but it's worth one
paragraph on what it costs. No vendor documents a feature as "this works as
long as the attacker hasn't read this page." No holder tells a reporter what
their backup scheme was. So when someone is abducted, or tortured for a
passphrase, or killed, the question *was this person relying on something
the attacker wasn't supposed to know?* has no recorded answer, because
nobody ever wrote one down.

So the obvious epidemiological question can't be asked. Doctors find
the cause of a disease by asking what the sick have in common. Here the thing
the victims might have in common is precisely the thing that is kept secret.
That's the first layer of the anosognosia, and it's the one the other three
sit on.

## Two: a homicide is reported as a homicide

When a holder is killed, the story is a murder. It isn't filed as a robbery
whose victim was then eliminated, and the bitcoin often never appears in the
coverage at all. So the cases that most directly show what
[the Deadly Race](https://zenodo.org/doi/10.5281/zenodo.22018891) predicts, a
holder killed because their being alive was in the attacker's way, are the
cases least likely to be recorded as attacks on holders.

This is the weakest of the four, and it's worth saying why before leaning on
it. It pushes the count of deaths down, but a matching silence pushes the other
side of the fraction down too. Someone who survives a wrench attack has every
reason not to tell the police, let alone a reporter, "I was tortured for my
bitcoin," because saying so tells the next crew where to go. So the one number
I keep citing, that 4.6% of recorded wrench attacks end in a death (16 of 351
in [Jameson Lopp's registry](https://github.com/jlopp/physical-bitcoin-attacks),
a press-sourced sample), is missing deaths and missing survivals, and nobody
can say which it's missing more of. It might be too low. It might be too high.

I'm keeping it on the list anyway, partly for completeness and partly because
what it does to the record is real even where its effect on one ratio washes
out: the killings that most directly show what the Deadly Race predicts are
the ones least likely to be filed as what they were.

## Three: the survivors were not told either

You'd think the first two could be worked around. If the victim is dead, ask
the family what they were running.

This is where it gets properly bleak. A scheme that depended on the attacker
not knowing depended on the holder not telling, and discretion isn't
selective. The family wasn't told either. That was the point.

And where they do know, telling costs them. Saying publicly that the victim
held bitcoin announces that someone in the house may hold it now, very often
the person saying it. So it gets withheld unless it might help catch someone.
The one person who could have answered the question is the one the theory
predicts won't survive to be asked, and the people left are the ones with the
least information and the most reason to keep what they have.

So: what the victims were running is censored by what vendors don't say. How
often the worst outcome happens is blurred by how it gets classified, in both
directions at once. And what's left is censored by what the bereaved don't
know or won't repeat. The part of the record that could tell you which designs
get people hurt is exactly the part that's missing. The disease has taken the
evidence of the disease, which is anosognosia in the strict, clinical sense.

## Four: conceding is expensive to whoever concedes

The first three remove evidence. This one removes the response to evidence,
and it's the part of the anosognosia that survives being diagnosed, which is
why writing this post doesn't dissolve it.

Suppose you accept the argument. What have you just said? If you're a vendor,
that a feature you shipped is worse than not having it, about devices already
in customers' hands. If you're a trainer, that the coached denial you sold
drains the credibility of everyone's denials. If you're a holder, that the
setup you're still running is the dangerous kind. The cost of agreeing is
private, immediate, and yours. The cost of not agreeing is spread across
holders you'll never meet, arrives later, and has no name attached.

That's the same shape as the problem in
[the Denial Spiral](https://zenodo.org/doi/10.5281/zenodo.22778480), one level up.
There, the shared resource being drained is how believable a denial is. Here
it's the field's ability to correct itself. In both, the sensible move for
each individual is to wait for someone else to go first. Stubbornness is
cheapest exactly where it's most expensive for everyone.

I should be careful about what this does and doesn't claim, because a theory
that predicts silence can be abused. It would be easy, and wrong, to read
every vendor who doesn't reply as secretly agreeing. People don't reply for
ordinary reasons: time, lawyers, disagreement they never wrote down. Nothing
here licenses a conclusion about any one of them. The prediction is about the
aggregate: that the analysis being available won't, by itself, get it adopted,
and that it'll be adopted first wherever conceding is made cheap. A neutral
name for the weakness. A reviewed paper to cite. A bar that was set before
anyone was measured against it.

## Vienna, 1847

Everyone reaches for Semmelweis here, and it's worth doing properly, because
the gesture version is a cliché and the real version is more useful.

In 1847 Ignaz Semmelweis was working in a maternity clinic in Vienna where
women were dying of childbed fever at a rate the midwives' clinic next door
didn't have. That spring his colleague Jakob Kolletschka cut himself with a
scalpel during an autopsy, and died of what looked exactly like childbed
fever. Semmelweis put it together: the doctors were coming straight from the
dissecting room to the delivery ward and carrying something on their hands.
He made them wash in chlorinated lime. Mortality in his clinic fell from
roughly 18% to roughly 2% within the year.

He was right two decades before germ theory could explain why, and he was
rejected anyway. Not only on the evidence, which was strong. On position. The profession's anosognosia had a very specific shape:
accepting it meant accepting that physicians' own hands had been killing their
patients. That's mechanism four exactly, and it's the only part of the analogy
I'll claim.

There's a second lesson in the story, and it cuts against me, so I'll take it.
When his book failed to persuade, Semmelweis started writing open letters
calling his critics murderers. It didn't help. What eventually changed practice
was Pasteur and Lister, twenty years on, giving the profession a way to agree
without having to confess, and the delay was counted in dead women. That's
why the Denial Spiral states a bar instead of an indictment,
classifies designs instead of people, and credits vendors where the record
credits them. Being right loudly is not the same as being right usefully.

## What kind of claim this is

At this point a fair reader asks: if every source of evidence is censored,
isn't this unfalsifiable? A theory that explains away its own lack of
evidence is usually a bad sign, and a theory of anosognosia is exactly the
kind that could.

It would be, if it were a claim about frequency. This is a claim about
structure, derived from what a rational attacker does given what he can and
can't know, in the way you can derive that a price ceiling produces queues
without counting any queues. No dataset could confirm it or refute it, and the
reason is internal to the subject: the only witnesses to an enacted case are
an attacker with every reason to deny the motive and a holder, or a family,
with every reason to deny the asset. Asking them isn't a weak instrument.
It's no instrument at all.

What it can be tested against is its own logic, and there are two specific
ways to break it. Show a setup where, after the attacker has the holder and
everything they carry, a path to the coins still exists but finishing it gives
the attacker no reason to want the holder gone. Or show that the attacker the
papers assume is, in some way that matters, weaker than a real one. Neither
needs a victim or a survey. Both are settled by reading the argument, and
either would sink it.

That's also why the papers end in a bar rather than a finding. Whether a
design leaves the holder as the last obstacle between an attacker and the
money is decided by reading the design. It doesn't wait on the data, and
it's just as well, because the data is not coming.

## Publishing anyway

So why write any of this, if the fourth mechanism says it won't work? Because
anosognosia in a field behaves differently from anosognosia in a brain.

The fourth mechanism is about cost, and cost can be moved. It
predicts that nobody wants to go first. It says nothing against making going
first cheaper: a named weakness class that isn't anyone's fault, a published
criterion you can apply to your own setup without anyone watching, papers with
DOIs that a vendor can cite as the reason for a change instead of admitting a
mistake. That's what this series has been trying to build. The only move the
fourth mechanism doesn't already price is to lay the argument out in public
and keep it there.

I should say where I stand in this. I sell security audits built on these
arguments, and the Great Wall project I work on is one answer to the bar the
Deadly Race sets. That's an interest, and you should weigh what I've written with it
in mind. I'd rather tell you than have you find it.

If you hold, the test is short and nobody has to see you take it. Suppose
someone has you, everything you carry, and a copy of your setup's manual. Is
there still a path to the bulk that only you can finish, given enough time?
If the honest answer is "yes, eventually," that path is what the Deadly Race
is about, and it only ever looked safe because nobody knew about it. You now
know about it.

---

*The four mechanisms, Semmelweis and the argument about what kind of claim
this is are in* [***The Denial Spiral***](https://zenodo.org/doi/10.5281/zenodo.22778480)*.
The criterion is in* [***The Deadly Race***](https://zenodo.org/doi/10.5281/zenodo.22018891)*.
Both open access, no signup.*

*Incident data from* [*Jameson Lopp's registry*](https://github.com/jlopp/physical-bitcoin-attacks)*,
a press-sourced sample: it misses what goes unreported and over-weights what made
the news. New cases I find go there rather than into a dataset of mine.*

---

**If this was worth your time.** Send it to whoever talked you into your current
setup. A ⭐ on [Great Wall](https://github.com/Yuri-SVB/Great-Wallet),
[the research](https://github.com/Yuri-SVB/great-wall-docs) or
[these posts](https://github.com/Yuri-SVB/great-wall-posts) costs nothing and
makes the work easier to find. And if you want to fund it,
[support](https://github.com/Yuri-SVB/support) takes ⚡ Lightning and on-chain, no
signup, no tiers, nothing expected back.
