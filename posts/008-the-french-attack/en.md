---
id: 008
title: "The (F/W)rench Attack"
subtitle: "A tax office database, queried for people who had declared crypto gains. Nobody found out through a crypto victim."
language: en
author: Yuri da Silva Villas Boas
papers: [DS, DR]
reading_time: ~6 min
cover: assets/cover-1200x675.webp
cover_alt: "A man in a beret and Breton stripes raises an adjustable wrench, a baguette and a glass of red wine under one arm, the Eiffel Tower behind him."
---

# The (F/W)rench Attack

<p align="center"><img src="assets/cover-1200x675.webp" alt="A man in a beret and Breton stripes raises an adjustable wrench, a baguette and a glass of red wine under one arm, the Eiffel Tower behind him." width="680"></p>

If you hold bitcoin in France and you declare it, you're in a database. In June
2025 an employee of the tax administration was taken into custody, accused of
querying that database for organized crime. Investigators reported the queries
covered, among others, people who had declared gains in cryptocurrency.

France is also where the wrench attack has become a national story, and this
post is about the connection between those two facts.

## A database, queried

### What the reporting says

The reporting describes an agent in Île-de-France consulting Mira, an internal tax
system holding sensitive files, with no professional reason to be in it. The
results, addresses and financial situations, allegedly went to a handler connected
to organized crime. Payment reportedly came by Western Union.

She's been in custody since 30 June 2025, under investigation for criminal
association and complicity in violence against a prison officer. At a hearing she
reportedly admitted the facts and declined to say who was giving the orders. The
proceedings are open and nothing here is a verdict.

The part that should bother you isn't any of that.

### How it surfaced, and why that is the worst part

The case came out because one of the addresses she passed on belonged to a prison
officer, and that officer was violently attacked. Somebody pulled that thread and
found the rest at the end of it.

So the crypto side wasn't found by a crypto victim reporting a break-in and an
investigator working backwards. It was found by accident, from a different crime
against a different kind of target. Which leaves a question nobody can answer: how
many queries left no thread for anyone to pull?

Not "probably a lot". Unknowable. That's the honest answer and it's worse than a
big number would be.

## The strongest version of the advice, taken seriously

Somebody always says, around here: fine, then don't create the record. Buy without
KYC. Declare nothing. Leave no trail.

That deserves taking seriously rather than waving off, because as personal hygiene
it's correct. Fewer records beats more records. If you've never been in a database
you have less to worry about than someone who has.

Three things stop it being a security mechanism.

## Exposure ratchets

The first is that it only ever pays in advance.

A record can't be uncreated. A leak can't be un-leaked. Whatever the exchange knew
about you in 2019 it knows permanently, and so does whoever has since obtained
what it knew. Whatever you declared is in Mira.

Which means the economics run against you from both directions at once. Staying
private compounds in cost: every year you hold, every counterparty you deal with,
every service that now wants a document. And it decays in value, because your
discretion is only worth something if nobody has published you already.

You pay more each year for something worth less each year. That isn't a defense
having a bad year. It's a defense with a direction.

Against a wrench attack France has made ordinary, that direction is the whole
problem: the people most exposed are the ones who have been holding longest.

## An offense, or a database that gets mined

The second is simpler and, for most people, settles it.

Where gains or holdings are legally reportable, "leave no record" isn't
discretion. It's non-declaration, which is a crime.

Taken literally, then, the advice is an instruction the law-abiding holder isn't
permitted to follow. You can be compliant or you can be invisible. Pick one.

And the usual reassurance, that the state's copy is at least safe, is what this
case is about. The compliant French holder did everything right, declared his
gains as required, and ended up in a file that was allegedly being queried to
order for people who wanted to know where he lived.

### One honest office, one dishonest employee

I want to be careful about the target. This isn't a story about a corrupt tax
administration. As far as the reporting goes it's one employee, and the case is
being prosecuted, which is the system doing its job. That's the point. A perfectly
honest tax office with one dishonest employee produces the same outcome for the
holder. The structural fact isn't the betrayal. It's that a queryable list of
people who hold bitcoin exists, and whether it stays shut depends on the integrity
of everyone who's ever had access to it, forever.

## Discretion was never a mechanism

The third reason makes the other two almost redundant, and it's a century old.

Kerckhoffs's principle: assume the attacker knows the system. Everything except
the key is public. You judge a design by how it performs against an adversary who
knows your situation, because sooner or later one does.

Discretion fails that by construction: it's a hope about the attacker's
ignorance rather than a mechanism. [*The Denial Spiral*](https://zenodo.org/doi/10.5281/zenodo.22778480) classifies the whole
shipped category that way, on the vendors' own documentation. And
[*The Deadly Race*](https://zenodo.org/doi/10.5281/zenodo.22018891) is what the hope costs you once it turns out to be
misplaced and you're the one in the room.

## The wrench attack, and the French attack

The man with the wrench at the top of this page is the joke in the title. I'd
rather explain it than leave it sitting there looking pleased with itself.

### The disproportion, and what it is made of

France accounts for 61 of the 351 incidents in Jameson Lopp's public registry of
physical attacks on bitcoin holders. That's 17.4% of everything recorded
worldwide, from a country with roughly 0.9% of the world's population. In 2026 it
accounts for something like two thirds of everything the registry logged.

The wrench attack is becoming the French attack.

<p align="center"><img src="assets/m1-france-share.png" alt="France accounts for 61 of 351 incidents in the wrench attack registry, 17.4% of everything recorded, from 0.9% of the world's population." width="680"></p>

And here's what has to travel with that line. It's a claim about what gets
recorded at least as much as a claim about what happens. The registry is built
from press reports. French wrench attacks became a sustained national news story
in 2025, which plausibly raises the rate at which French cases enter the registry
at all, independently of how many occur. A country whose press covers this
intensely looks worse than one whose press doesn't, and some of that gap is
journalism rather than crime.

### What the data can't settle

So France dominates what's recorded. How much is incidence and how much is
visibility is exactly the question someone with non-public French data could
answer and this dataset can't. If that's you, I'd like to hear from you.

What isn't in doubt is the shape. Organized crews, reconnaissance, targets picked
off lists, including here a list the state was keeping because the law told it to.

The counsel says keep a low profile. The law says declare your gains. Pick one.

The file says it already knows.

---

*Two papers sit behind this.* [***The Denial Spiral***](https://zenodo.org/doi/10.5281/zenodo.22778480)
*classifies the defenses that rest on an attacker's ignorance, and shows why the
advice gets worse for everyone the more people follow it.*
[***The Deadly Race***](https://zenodo.org/doi/10.5281/zenodo.22018891) *is what it costs you
when one of them fails: a seizure that leaves a feasible-but-unfinished path
turns a robbery into a race, and prices your elimination. Both free, no signup.*

*Incident data from* [*Jameson Lopp's registry*](https://github.com/jlopp/physical-bitcoin-attacks)*,
a press-sourced sample: it misses the unreported and over-weights whatever made
the news. New cases I find go upstream there rather than into a database of mine,
which in a post about databases seems worth saying out loud.*

---

**If this was worth your time.** Send it to someone who still thinks silence is a
plan. A ⭐ on [Great Wall](https://github.com/Yuri-SVB/Great-Wallet),
[the research](https://github.com/Yuri-SVB/great-wall-docs) or
[these posts](https://github.com/Yuri-SVB/great-wall-posts) costs nothing and makes
the work easier to find. And if you want to fund it,
[support](https://github.com/Yuri-SVB/support) takes ⚡ Lightning and on-chain, no
signup, no tiers, nothing expected back.
