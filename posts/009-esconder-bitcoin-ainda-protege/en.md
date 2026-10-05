---
id: 009
title: "Does Hiding Your Bitcoin Still Protect You?"
subtitle: "Brazil has the world's worst statistic for the kind of attack where hiding doesn't help, and the market keeps selling hiding places."
language: en
author: Yuri da Silva Villas Boas
papers: [DS, DR]
reading_time: ~7 min
translation_of: pt-BR.md
cover: assets/capa-1200x675.webp
cover_alt: "A man holds a sieve up to block out the sun, and the light pours straight through the mesh. It is the Brazilian idiom for trying to hide what everyone can already see."
---

# Does Hiding Your Bitcoin Still Protect You?

<p align="center"><img src="assets/capa-1200x675.webp" alt="A man holds a sieve up to block out the sun, and the light pours straight through the mesh. It is the Brazilian idiom for trying to hide what everyone can already see." width="680"></p>

**The standard advice for anyone afraid of being kidnapped over bitcoin comes in
three parts: tell nobody, deny it if asked, and keep a *decoy* to hand over.**

**All three are bets on what the criminal will *believe*. And not one of them has
ever been assessed as what it is: a security mechanism whose entire strength rests
on the adversary's ignorance.**

This piece argues that hiding bitcoin isn't merely ineffective. It's **self-destructive at
scale**, and the bill lands on people who never took the advice.

---

## Hiding bitcoin has a name, a number and a rap sheet

The vocabulary first.

A *decoy*, or bait wallet. In Brazil we call it "the mugger's money", and we know
it well: a smaller amount, set aside on purpose to be handed over in a robbery.

In security engineering the whole family of these tactics is cataloged. It's
called *Reliance on Security Through Obscurity*, filed as
[CWE-656](https://cwe.mitre.org/data/definitions/656.html). In any other domain
that's a design defect. In bitcoin custody, it's the consensus.

### Hiding bitcoin is condescending by construction

This paradigm, which in protocol design is called **obscurity**, is intrinsically
condescending. It assumes the thief isn't mentally capable of reading the same
manuals, watching the same tutorials and taking the same courses as his victims.

If you can learn a procedure on the internet, so can a thief. And he'll certainly
know the procedure exists.

---

## Brazil sits in the registry's worst quadrant

Jameson Lopp has kept a [public registry of physical attacks on bitcoin
holders](https://github.com/jlopp/physical-bitcoin-attacks) for years, the "$5
wrench attacks". I coded all 351 incidents in it by modality. The country
breakdown isn't uniform: it varies by an order of magnitude.

| Jurisdiction | Incidents | Kidnapping | Armed robbery | K:R ratio |
|---|---:|---:|---:|---:|
| **Brazil** *(small n)* | 12 | 75.0% | 8.3% | **9.0** |
| France | 61 | 57.4% | 8.2% | 7.0 |
| *All incidents* | 351 | 35.0% | 22.8% | 1.5 |
| United States | 59 | 20.3% | 33.9% | 0.6 |
| Russia *(small n)* | 10 | 30.0% | 50.0% | 0.6 |

### Nine kidnappings for every robbery

Read the right-hand column. In the United States the typical attack is a robbery:
gun drawn, immediate transfer, minutes on scene.

In Brazil the proportion inverts. **For every armed robbery on record, nine
kidnappings.**. The Brazilian attack isn't an event of minutes. It's an event of
hours or days, with the victim under the criminal's control throughout.

### The caveat comes with it, and it's serious

The registry is a press-sourced sample, `n=12` for Brazil supports nothing on its
own, and the coding is by headline keyword, not by measured duration. Treat the
Brazil row as directional.

The comparison that actually carries weight is France against the United States:
two subsets of the same size (61 and 59) with inverted compositions. Composition
does vary with local conditions, and Brazilian local conditions are known to
anyone who lives here.

This matters because **the whole promise of hiding bitcoin depends on the attack being
short**. A decoy works if the criminal takes the R$8,000 and leaves. It has no
answer to the next question, asked on the third day, in captivity.

---

## What happens when everyone is trained to deny

Here's the mechanism, and it's economic before it's cryptographic.

### A denial's credibility is a common resource

It's produced by the set of all holders and consumed by each one who denies. While
denial is rare, denying carries information: the criminal updates his belief and
your odds of being released go up.

Once denial becomes the expected script, once every channel, every course, every
Telegram group teaches the same line, **a denial stops carrying information**.

An interrogation that opens with "I don't have anything" gives the criminal no
update in your favor. And his rational continuation at that point isn't to let
you go. It's to press.

The individually rational response to that environment is to hide better and
rehearse more. Which **depletes the resource further, for everyone**.

I've called this the **Denial Spiral**, and its cost is a classic externality: it
falls on whoever needs to be believed. Including people using an arrangement that
doesn't depend on lying. Including people who honestly **hold no bitcoin at all**,
and the registry has cases like that.

### The market sells the depletion as a product

Various self-custody consultancies, courses and tutorials list, among their paid
services, setting up decoys with credibility training.

So: you pay to become fluent in a denial that the criminal already discounts,
precisely because it's taught and sold. The remedy degrades the very thing it
sells, and not only for the customer.

---

## The worse problem: you cannot prove you forgot

There's a second failure, and it's worse, because it's about the outcome rather
than the duration.

Start from a simple, inescapable fact: **nobody can prove they don't know
something.** Knowing is demonstrable; *not* knowing isn't. You have no way to prove
you forgot the passphrase, or that no backup exists anywhere.

### The Deadly Race

Now consider any scheme that, after your device is taken, leaves the criminal with
a **feasible but unfinished** path to the money: a timelock, a delegate-held
recovery, a vault with a delay, a key that still has to be cracked.

You're released. And you can't prove you kept no usable copy.

What exists from that point is a **race** between you and him for the same balance.
And a race against a competitor who is within arm's reach creates something no
wallet whitepaper mentions: **a material incentive to eliminate you.** Not out of
cruelty. Out of arithmetic. Taking the other racer off the track is the cheapest
move available.

I've called this the **Deadly Race**. In the registry, at least 4.6% of incidents
(16 of 351) involve a victim killed, and that figure is a **floor**, not an
estimate. A homicide tends to be reported as a homicide, not as "attack on a
bitcoin holder". The outcome the argument predicts is documented in practice.

### Why the decoy is a gray-zone machine

The design criterion that falls out of this is blunt: **a coercion-resistant
custody scheme can admit only two outcomes. The attack clearly works, or the
attack clearly fails. Never a race.**

The gray zone is exactly where the incentive to murder lives. I've called this the
**No-Gray-Area Principle**.

Notice what that does to the decoy. It is, by construction, a gray-zone machine:
the criminal leaves suspecting there's more, with no way to settle the suspicion.
It's the worst possible place to be.

---

## A Brazilian case that closes the argument

Porto Velho, October 2019. A gang kidnaps
[Arcilio Nogueira de Souza](https://archive.is/jyzcJ), ties the victim to a tree
and beats him for hours. The criminals **took nothing**. The phone gave no access
to the funds.

That case is the whole argument in one paragraph. The funds being inaccessible
*did not end the attack*. It **prolonged** it.

The scheme "worked" in the sense the industry measures, the money didn't move, and
the person spent hours tied to a tree being beaten, because outside his head
there was nothing that could settle the criminal's doubt.

This is why I separate the two mechanisms. The Deadly Race prices the **outcome**.
The Denial Spiral prices the **duration**. An arrangement can be innocent of one
and guilty of the other, and most of what's sold today is guilty of both.

---

## What's left, if hiding bitcoin isn't a defense

Three honest routes remain, and it's worth knowing which one you're on.

### 1. Physical

Geographic dispersion, vaults, multisig with distant custody. It works, and it
reduces bitcoin's security to "how good is the vault". Bitcoin becoming **gold
with extra steps**, at a cost that scales with the defense. For the vast majority,
it's out of reach.

### 2. Delegated

Someone beyond the criminal's reach holds the missing piece: an exchange,
co-custody, third-party recovery. It clears the criterion, but it swaps the
premise: custody stops being individual. *Not your keys.* And the route **closes**
if the delegate lives near you.

### 3. Tacit

The secret was never on the device, and can't be dictated even under torture,
because it's perceptual recognition rather than a phrase. Seizing the hardware
yields nothing feasible. **Clear failure**, no racer left over, custody still
individual.

The third route is where I work, and the project is called **Great Wall**. Here's
the warning any honest text about it needs: **the implementation is a prototype.
Don't put your savings behind it yet.**

When that changes it will be written down, with a date, in
[`DELIVERED.md`](https://github.com/Yuri-SVB/support/blob/main/DELIVERED.md), a
file kept in git precisely so that "the work is progressing" is an auditable claim
and not a promise.

### The counterintuitive side effect

There's a nice side effect to this route: **a public, non-obscure project improves
the position of people who deny.**

A criminal who believes an effective mechanism is in circulation is believing that
lying isn't the victim's only available tool, and a victim with a real
alternative has less reason to lie.

Hiding remains bad as a primary defense. But which arrangement it accompanies is
not a matter of indifference.

---

## What I sell, and what I don't

**I don't sell software.** Great Wall, BTC-D20, BIP-450 and the papers are MIT or
Apache-2.0, and that doesn't change: no "pro" version, no feature unlocked by
payment, no priority queue for donors.

It's written down in the [support repository](https://github.com/Yuri-SVB/support),
and it's written there because a promise in an article is worth nothing and a
promise in git has a date.

### I do sell self-custody consultancy

It's a service, and the service is this: I look at the arrangement you already have,
hardware wallet through passphrase, multisig, decoy, inheritance plan, whatever
there is, and answer four questions in a closed report:

1. Does your security rest on a **secret trick**? Does it depend on the attacker
   not knowing what you do, and how you do it?
2. Once your devices and secrets are seized, could the attacker spend **right
   away**, or only **eventually**? "Eventually" means you're still a racer.
3. Is your custody **strictly individual**? Can anyone else do something that
   stops you reaching your own coins?
4. Does it depend on **particular objects in particular places**? And do you own
   those places?

It isn't product sales: in most audits the recommendation is to adjust what already
exists, and in some the verdict is that it's reasonable. What I won't do is build a
decoy with denial training, for the entire argument above.

Contact: **yuri@t3infosecurity.com**.

### And if you don't want to buy anything

The papers are free and behind no signup:
[*The Deadly Race*](https://zenodo.org/doi/10.5281/zenodo.22018891) (the race and the
criterion) and [*The Denial Spiral*](https://zenodo.org/doi/10.5281/zenodo.22778480) (the
spiral, the classification of obscure products on the market, and the registry
coding method).

New incident data goes to [Lopp's registry](https://github.com/jlopp/physical-bitcoin-attacks)
rather than into a database of mine, because that information is a public asset and
belongs to everyone, including whoever is next.

If this was useful, [support lives here](https://github.com/Yuri-SVB/support).
Lightning and on-chain, nothing expected in return and no signup.

---

*Yuri da Silva Villas Boas is an applied cryptographer, author of BIP-450 (Formosa)
and of the Great Wall protocol. The two central claims in this article are
developed formally in the papers cited, currently under academic review.*
