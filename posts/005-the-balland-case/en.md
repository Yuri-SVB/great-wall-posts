---
id: 005
title: "The Balland Case — an Embarrassment to the Self-Custody Creed"
subtitle: "A co-founder of Ledger was seized from his home and mutilated. What got him out was the state and a centralized issuer, and both of those are outside the creed."
language: en
author: Yuri da Silva Villas Boas
papers: [DS, DR]
reading_time: ~9 min
cover: assets/cover-1200x675.webp
cover_alt: "A hand holding a pair of old pliers in near-darkness, one hard light across the knuckles, beside a panel reading The Balland Case, an embarrassment to the self-custody creed. The panel states that the picture is merely illustrative: a staged photograph of a hand tool, not his case, not the attackers, and not a claim about what was used."
---

# The Balland Case — an Embarrassment to the Self-Custody Creed

<p align="center"><img src="assets/cover-1200x675.webp" alt="A hand holding a pair of old pliers in near-darkness, one hard light across the knuckles, beside a panel reading The Balland Case, an embarrassment to the self-custody creed. The panel states that the picture is merely illustrative: a staged photograph of a hand tool, not his case, not the attackers, and not a claim about what was used." width="680"></p>

In January 2025 men took David Balland out of his home. Balland co-founded
Ledger, which makes hardware wallets, which means that of all the people in the
world he was among the most likely to have thought carefully about how his
bitcoin was held.

They took his wife too. They cut off one of his fingers and sent it, to make the
point that the demand was serious. He was freed by an elite unit of the French
national police. His wife was freed roughly a day later. A ransom had been paid
by then, not by Balland but by an associate of his, and most of it was recovered
afterwards because part of it had moved through a centralized stablecoin whose
issuer could freeze it on request. Something like 5% never came back.

One thing in that paragraph is independently checkable. An issuer freeze leaves a
public record. The rest of it, meaning who paid and how much and how the
recovery went, rests on the accounts of the people involved, and I have no way
to audit those.

## What actually got him out

Sit with the shape of it rather than the horror of it for a moment.

A professional champion of self-custody was attacked anyway, with presumably the
best self-custody setup money and expertise can assemble. Wealth did not prevent
it. Prominence did not prevent it. Expertise in exactly this problem, of
the kind almost nobody else has, did not prevent it.

And when it was over, the two things that undid the damage were **an elite state
police unit** and **a centralized issuer with a freeze button**. Neither of those
is part of the creed. Both of them are, on most days, things the creed exists to
route around.

That is what makes the case worth writing about, and it is also why it is
uncomfortable. If you argue for self-custody, as I do, this is the case you have
to be able to look at without flinching.

**The lesson is not that Balland erred.** I want to be exact about that, because
the reflex in this space is to read every incident as a competence story. He
should have used multisig, he should have moved, he should have kept quieter.
Nothing published suggests he did anything wrong, and the argument here does not
need him to have.

## What his setup could and could not touch

Nothing about Balland's self-custody setup had any bearing on whether men came
to his house. Target selection runs on what is visible from outside: a name, a
company, a public role, a database somebody leaked. No wallet configuration
touches any of that.

Nor did it set how long they stayed, and this is the place where people like me
oversell the argument. Start from the impossibility both papers rest on. You
cannot prove you forgot, so an attacker in the room assumes there is more, and
he assumes it whatever you built and whatever you tell him. From there the
length of the encounter is his arithmetic and not yours: another hour either is
or is not worth its risk to him. A protocol is a set of virtual objects and
rules for using them. It does not stop a wrench.

What a self-custody design can be held to starts earlier than any of that, with
describing the attacker honestly. The model the papers work from puts one clause
first, before anything about compute or budgets: he knows how your setup works.
Reading the manual is free and the manual is public, so assume he has. That is
the ground [***The Denial
Spiral***](https://zenodo.org/doi/10.5281/zenodo.22778480) covers, and it is
where an entire product category fails, because decoys and duress PINs and
coached stories all need him not to have read it. Obscurity did work once, which is what
[an earlier post in this series](https://github.com/Yuri-SVB/great-wall-posts/tree/main/posts/003-the-window-has-closed)
is about: there was a window in which almost nobody was looking for you and
nobody could pick you out of a crowd, and inside it staying quiet was close to a
complete defense. It is worth saying why the culture holds onto that rather than
sneering at people for it. But knowledge spreads (Kerckhoffs), and a criminal business model that
pays gets replicated (Mises). The window closed and it is not reopening.

Model him that way and something unpleasant surfaces. Some arrangements, run
against an attacker who knows exactly what they are, hand him a reason to kill
you that he would not otherwise have had. That is what
[***The Deadly Race***](https://zenodo.org/doi/10.5281/zenodo.22018891) prices: when the path
he holds still works but is not finished, the freed holder is a competitor for
the same money, and a competitor within reach is cheaper to remove than to
outrun. Balland was released alive, so that move never arrived here. The point is
that some designs manufacture it, and the Deadly Race's name for that class is
*worse than useless*. The phrase is narrow on purpose: a scheme that hands
everything over cleanly beats a scheme that leaves a gap. Before trying to help,
do no harm.

Only with both of those in hand is the question everybody starts with worth
asking, which is how much of the stash can be put out of reach, and the second
half of that question is the part people skip: without buying the reduction at
the price of a race.

What that buys is smaller than the version people want, and getting its size
right takes the rest of this piece.

None of this is an argument against self-custody, and it would be a cheap one if
it were. It is an argument about the order you do things in: describe the
attacker as someone who has already read your manual, notice which of the things
you could build would price your own death, and only then start asking how much
you can put beyond reach.

## Why no search ever ends

Both papers reason about a deliberately unflattering attacker. He knows how your
setup works, he has a budget of time and risk, and he assumes there is always
more to get. Call him the idealized one. A design has to survive him, because a
design that only survives a careless opponent has not survived anything.

For him there is a question he cannot answer and cannot stop asking.

Is there another copy?

**You cannot prove you forgot.** You cannot prove a backup does not exist either,
and the reason is not that the attacker is stupid or sadistic. It is that the
thing he would need to rule out is tiny and can be anywhere. An SD card.
Steganographic notes in a book on a shelf. The memorized login and password of an
email account holding an encrypted file. Any of those is enough to reconstitute
access, and none of them can be excluded by searching a house.

So he assumes one exists, whatever you say, however you say it. That is the
rational position, not the paranoid one.

Follow it one step further and you arrive somewhere the Deadly Race does not
flinch from. To be certain no copy remains, he would have to establish what is
and is not in your memory. Orwell gave the last private place its measure:
*nothing was your own except the few cubic centimetres inside your skull.* An
attacker who could read that would exceed the literary supremum of surveillance
power, which expressly conceded the skull.

That is the end of the road the design puts you on, for that attacker. Hold
onto the qualifier, because it does more work than it looks.

## The person they take is not always the person who holds

An associate paid. Not Balland, and not out of Balland's own arrangement. That
detail is easy to read past and it is the second argument of the case.

Hand-coded from Jameson Lopp's registry: in **12 of 351 incidents, 3.4%**, the
person seized was not a holder at all but a relative taken to compel one. A
parent, a spouse, an adult child. The screen surfaced sixteen candidates and four
were discarded on reading, including one where "son of" turned out to name a
perpetrator rather than a victim, so the twelve are audited rather than
keyword-matched.

Two things about that subset matter more than its size.

It is **recent and concentrating**. Eleven of the twelve fall in 2023 or later,
and nine of them are in France, where recorded incidents went from about one a
year through 2024 to 22 in 2025 and 34 by August 2026. Whatever part of that rise
is real incidence rather than the French press paying attention, this is not a
historical scatter. The tactic is being adopted.

And 3.4% is a **floor**, not an estimate. The coding reads a one-line headline, so
an incident that does not happen to mention a relative is no evidence that none
was involved. The number can only be understated.

## What that bounds

The delegated arrangement is a real answer to coercion, and the honest thing is
to say so before taking anything away from it. It is also the point where
self-custody quietly stops being self-custody. Put the power to release funds with someone far away who will
refuse you, and an attacker in your living room has nobody to profitably hurt.
It clears the bar. The [companion post](https://zenodo.org/doi/10.5281/zenodo.22018891)
says so plainly.

What this case prices is the fine print. That arrangement works only while the
delegate is genuinely out of reach, and the delegate a real person actually
appoints is a spouse, a parent, an adult child, a trusted associate. Which is the
exact list this subset shows being seized.

So a reachable delegate is not a second racer. It is a second victim.

The route is not refuted, it is bounded: it needs unreachability that is
**structural** rather than assumed, and most people who think they have that have
assumed it. Ask who you would actually name, then ask whether that person could
be found in an afternoon by somebody who already found you.

## The attacker in the model is not the attacker in the room

The idealized attacker never stops, and that is the whole point of him. Real ones
stop all the time, for ordinary reasons: a budget, a risk of being caught that
grows by the hour, an arithmetic about the next hour rather than about the whole
prize.

A real one can also be *informed*, which the idealized one never needs to be.
Three things he can come to know, none of which require him to believe anything
the person in front of him says:

1. **That such a construction exists.** Not a claim the victim is making, a
   public fact about what is available to build with.
2. **That people holding a lot plausibly use it**, and so do their relatives, for
   the bulk of what they hold between them.
3. **So the expected value of another hour falls**, and with it the expected
   value of starting at all.

That is not a promise, and the hedge still stands: someone wealthy enough has a
smaller, looser, less guarded portion, and in the attacker's arithmetic that
alone can cover the risk of the crime. What moves is the arithmetic on the bulk.
A hypothetical Balland whose self-custody cleared all three could still have been
picked out, still have been taken, and his relatives could still have paid
whatever was reachable. What would be different is what his attackers could
eventually establish: that the rest is out of operational reach as a property of
the construction, rather than as a story he is telling them.

Design for the attacker who never stops. Deterrence runs through the one who
does.

## What is left

Against a determined attacker willing to hold you for a long time, the
self-custody options being sold today collapse to two: a state rescue, and an issuer willing to freeze.
Both worked here. Neither is self-custody, and neither is something you can
requisition when you need it. A creed whose fallback is other people's
institutions is not the self-sufficient thing it is sold as.

The alternative worth building is not better recovery after the fact. It is
removing the leverage in the first place — no standing device to seize, no token
that functions as a hostage, no delegate positioned to pay. Whether that is
achievable is the claim the papers make and defend, and you should read them
skeptically rather than take it from a blog post.

Balland got most of his money back and kept his life. He did not get the finger
back. That is the part of the ledger nobody freezes.

---

*The case, the proxy-victim subset, the audit behind it and the duration argument
are in* [***The Denial Spiral***](https://zenodo.org/doi/10.5281/zenodo.22778480)*, open
access, no signup. Its companion,*
[***The Deadly Race***](https://zenodo.org/doi/10.5281/zenodo.22018891)*, is where the
impossibility that makes a denial unverifiable, and the test it yields, are
developed properly.*

*Case details from* [*DL News*](https://www.dlnews.com/articles/regulation/ledger-cofounder-david-balland-and-wife-kidnapped-in-france/)*,
[archived](http://archive.today/2026.09.03-171044/https://www.dlnews.com/articles/regulation/ledger-cofounder-david-balland-and-wife-kidnapped-in-france/).
Incident counts from* [*Jameson Lopp's registry*](https://github.com/jlopp/physical-bitcoin-attacks)*,
a press-sourced sample that misses what goes unreported. Nothing here goes beyond
what was reported.*

---

**If this was worth your time.** Send it to whoever told you a hardware wallet
was the end of the problem. A ⭐ on [Great Wall](https://github.com/Yuri-SVB/Great-Wallet),
[the research](https://github.com/Yuri-SVB/great-wall-docs) or
[these posts](https://github.com/Yuri-SVB/great-wall-posts) costs nothing and
makes the work easier to find. And if you want to fund it,
[support](https://github.com/Yuri-SVB/support) takes ⚡ Lightning and on-chain, no
signup, no tiers, nothing expected back.
