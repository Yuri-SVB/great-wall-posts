---
id: 001
title: "From Magic Internet Money to Gold With Extra Steps"
subtitle: "Holding your own bitcoin now carries roughly the cost of renting a vault. Nobody quotes you that price, which is the only reason it doesn't feel like one."
language: en
author: Yuri da Silva Villas Boas
papers: [JUSTIFICATION, DR]
cover: assets/cover-1200x675.webp
cover_alt: "The gymnastics meme. On the top beam a gymnast simply walks across, labeled Buy Gold and Protect it Physically. Underneath, a row of contortions on the bars, the horse and a burning car, labeled with the self-custody ritual: roll 666 dice, follow weekly hack news, take a cyber security course, install TailsOS, multi-sig, multi-vendor, multi-location setup, train your family, buy an inheritance plan consultancy, keep profile low, tell nobody about Bitcoin. The panel beside it reads Gold With Extra Steps, and states that the comparison is about what it costs to keep the thing safe and nothing else, that it is not a claim that metal is good money, and that the rate comes from a registry built out of press reports and is therefore a floor."
---

# From Magic Internet Money to Gold With Extra Steps

<p align="center"><img src="assets/cover-1200x675.webp" alt="The gymnastics meme. On the top beam a gymnast simply walks across, labeled Buy Gold and Protect it Physically. Underneath, a row of contortions on the bars, the horse and a burning car, labeled with the self-custody ritual: roll 666 dice, follow weekly hack news, take a cyber security course, install TailsOS, multi-sig, multi-vendor, multi-location setup, train your family, buy an inheritance plan consultancy, keep profile low, tell nobody about Bitcoin. The panel beside it reads Gold With Extra Steps, and states that the comparison is about what it costs to keep the thing safe and nothing else, that it is not a claim that metal is good money, and that the rate comes from a registry built out of press reports and is therefore a floor." width="680"></p>

Think about what self-custody actually asks of you now.

Roll dice, because you don't trust a device's entropy. Stamp the words into steel,
because paper burns. Never say the word bitcoin at a dinner party. Keep a second
wallet with a plausible balance, in case someone asks you at knifepoint. Read
every hack post-mortem, in case it's your firmware this time.

That's not a monetary system. That's a security regime, and security regimes have
prices.

## Somebody already worked out the price

Insurers have been putting a number on "portable, valuable, and stealable" for
about two centuries. Jewelry, watches, collectible cars. Six independent sources
converge on the same figure: 1 to 2 percent of appraised value per year in the
United States, with the pure premium net of admin loading around 0.9 percent.

That's the market's own estimate of what physical vulnerability costs, and it's
not a guess. It's priced by people who lose money when they get it wrong.

You can run bitcoin through the same machinery. Take the wrench-attack rate
against individual holders, scale it by the insurance industry's own coefficient
for crime rate to premium, and adjust for the two ways a wrench attack is worse
than a burglary: it usually takes the whole wallet rather than some of the
jewelry, and you can't insure it, so you carry the tail yourself.

I get **about 0.55 percent a year** for individual holders above $100K, on 2026's
pace as of the August registry snapshot.

Institutional gold storage runs 0.5 to 1.5 percent.

## Where that number comes from, and what's wrong with it

The rate comes from [Jameson Lopp's public registry of physical
attacks](https://github.com/jlopp/physical-bitcoin-attacks), coded at commit
`9a4a62a`: 351 incidents, 1 in 2014, 85 in 2025, 53 in 2026 through mid-August,
which annualises to about 86. Thirteen of those 351 are ATM or crypto-machine
incidents rather than attacks on a holder. Dropping them changes the total to 338
and the recent years barely at all, so I've left them in and told you they're
there.

The registry is built from press reports. It misses everything unreported and
over-weights whatever made the news, so the count is a floor with an unknown
ceiling. Then a multiplier for underreporting, which I've set at 3, the most
conservative value anyone uses. And a severity multiplier of 6, being 3 for
total-versus-partial loss times 2 for bearing uninsurable risk.

Both of those are stipulations. Move them and the number moves: at the
underreporting estimate the registry's own maintainer thinks is closer to true,
it lands north of 2 percent. I'm publishing the low end on purpose. If the
conservative number already embarrasses the thesis that self-custody is free,
there's no need to argue about the aggressive one.

## What that actually means

Bitcoin's pitch was never that it would be cheap to hold. It was that holding it
wouldn't require anyone's permission or anyone's building.

Gold's problem was never that gold is bad money. Gold's problem is that a
meaningful amount of it has to live somewhere, and somewhere has a landlord, a
jurisdiction, and a guard who knows the combination.

So when the cost of holding bitcoin yourself converges on the cost of vaulting
metal, something has gone wrong that a price chart won't show you. You're paying
gold's carrying cost. You're just paying it in dice rolls, steel plates,
silence and vigilance instead of a monthly invoice, which is why nobody
experiences it as a fee.

The invoice arrives all at once, to one person, on one bad evening.

## The obvious objection

Geography fixes this, and I want to be fair to it, because it genuinely does clear
the bar.

Split the keys. Multisig across three countries. A vault in one, a trusted
relative in another, a safe deposit box in the third. An attacker at your door
now can't finish the job, so the attack doesn't pay.

That works. It also costs money that scales with how well it works — more sites,
farther apart, better guarded — and it re-answers the question "is my money safe?"
with "how good are my physical defenses?", which is the exact question Bitcoin was
supposed to retire.

You've rebuilt the vault. It's just distributed now, and you're the one
commuting between the branches.

## So buy the metal?

If you've read this far and concluded the sensible move is to hold something
physical and guard it properly, I'm not going to pretend that's irrational.
Measured against self-custody as it is actually practiced today, it isn't.

Be careful what that concedes, though, because it's narrower than it sounds. I'm
not telling you metal is good money, and nothing above argues that it is. The
claim is a comparison, on one axis only: what it costs you to keep the thing
safe. On that axis the mainstream advice, which is a device in a drawer, words
on steel, a rehearsed denial and a wallet kept small enough to hand over, has
lost whatever lead it had. The two papers behind this post are about why that
advice fails, and neither of them is about gold.

Here, I'll even save you a search:
[Morgantis Metais](https://morgantis.com/?utm_source=great-wall-posts&utm_medium=article&utm_campaign=001).
Avelino Morgantis has spent years arguing in Brazilian Bitcoin circles that metal
beats magic internet money, and on the specific question of carrying cost he has
been right the whole time. That's not a concession I enjoy making and it's not a
joke at his expense. It's the argument of this post.

What I dispute is that those are the only two options.

## The third thing

Physical distribution clears the bar by making the attack too expensive. Delegated
custody clears it by putting the deciding party out of reach, at the cost of the
thing being yours. Both work. Both cost you something Bitcoin was meant to give
you back.

The route I work on, [Great Wall](https://github.com/Yuri-SVB/Great-Wallet), clears it a
different way: the secret isn't on any device and isn't something you could hand
over under duress, because it isn't a phrase. So
there's nothing at the house worth taking, no guard to pay, no branch to commute
to, and no relative holding a piece.

It's a prototype. Don't put savings behind it yet. When that changes it'll be
dated in public.

But the reason I'm building it is in the number at the top of this post. A
cryptographic problem got solved a long time ago and then quietly turned back into
a physical one, and almost nobody is pricing it, because the price doesn't arrive
as a bill.

---

*Full model, with every parameter and source:*
[***The Security Tax***](https://github.com/Yuri-SVB/great-wall-docs) *(economic
analysis).* *The threat model behind it is*
[***The Deadly Race***](https://zenodo.org/doi/10.5281/zenodo.22018891)*, with its
companion* [***The Denial Spiral***](https://zenodo.org/doi/10.5281/zenodo.22778480)*.
Free, no signup.*

*Incident data from* [*Lopp's registry*](https://github.com/jlopp/physical-bitcoin-attacks)
*at commit* `9a4a62a`*, coded by a script in the paper's source tree so you can
re-run it and disagree with me precisely. New cases I find go upstream there.*

---

**If this was worth your time.** Send it to someone who thinks self-custody is
free. A ⭐ on [Great Wall](https://github.com/Yuri-SVB/Great-Wallet),
[the research](https://github.com/Yuri-SVB/great-wall-docs) or
[these posts](https://github.com/Yuri-SVB/great-wall-posts) costs nothing and makes
the work easier to find. And if you want to fund it,
[support](https://github.com/Yuri-SVB/support) takes ⚡ Lightning and on-chain, no
signup, no tiers, nothing expected back.
