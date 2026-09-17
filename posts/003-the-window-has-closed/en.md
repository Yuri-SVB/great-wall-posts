# The Window Has Closed

**Four things used to be true about getting robbed for your bitcoin. None of them
are true anymore, and none of them are coming back. Almost all of the advice you
have been given about protecting yourself was calibrated for the world in which
they were true.**

![The four conditions that made early holding safe, with identification struck out. A claim about incentives, not a measurement.](assets/m1-four-panes.png)

---

## There was once a time

Think about what had to go right for you, back then, for a wrench attack to not
happen.

**First, most thieves had no idea what bitcoin was.** Not "underestimated it" — had
never heard the word. The category of criminal who could even form the intention
to rob you of a private key was vanishingly small.

**Second, even the ones who knew were unlikely to ever meet you.** There were not
many holders. Encountering one by chance, in the course of an ordinary burglary,
was a coincidence that mostly did not happen.

**Third, and this is the one people forget: they had to know it was you.** Meeting
a holder is not the same as identifying one. Without a way to tell holders from
everyone else, knowledge of bitcoin buys a thief nothing. It is a capability with
no targeting.

**Fourth, if all three failed and someone did come for you, you probably knew more
than they did.** The early holder was typically a cypherpunk, a cryptographer, someone 
who had read the mailing list. The attacker was typically an amateur with a plan he 
had improvised that week. The technical asymmetry would tend to run in the victim's
favour.

That was a real window, and it was genuinely quite safe in there.

## What replaced each of them

Take them in order.

**Everybody knows what bitcoin is.** That one needs no argument.

**There are a great many holders.** Also no argument needed.

**And now they can tell it is you.** This is the one that actually changed the
game, and I will come back to it in a moment, because it deserves its own section.

**And the asymmetry has flipped.** The people doing this are not improvising.
French prosecutors have charged 88 people across a dozen linked kidnapping and
extortion cases — that is not a run of opportunists, that is organisations, with
reconnaissance, division of labour, and repeat business. Meanwhile the holder they
come for is now, statistically, a normal person who bought some bitcoin on an app.
The cryptographer-versus-amateur matchup has become something closer to its
opposite.

You can watch the shift in the shape of the attacks, too. In one industry count of
the first half of 2026, reported **home invasions** went from **1 to 20** out of 52
incidents year on year. The attack is moving to where people live. That is not the
profile of a crime of opportunity.

![Reported home invasions rose from 1 to 20 of 52 incidents year on year. Industry count; verified incidents only, press-sourced, directional.](assets/m6-home-invasions.png)

On counts generally: there are several available series for how many of these
happen per year, they disagree with each other about the exact numbers, and they
agree completely about the direction — a handful a year before 2017, dozens a year
now. I would rather tell you that than pick whichever number is most alarming and
present it as settled. The registries are built from press reports, so they miss
everything unreported and over-represent whatever made the news.

## The target list is public now

Here is the part that closed the window for good.

For a thief to target you specifically, they need a list. For most of bitcoin's
history there was no list. Now there are many, and you did not consent to a single
one of them.

Threat-intelligence reporting on the 2026 wave attributes victim selection to
leaked databases, tax records, and exchange data — plus insider sales of customer
lists and dark-web recruitment of employees with database access. Chain analysis
sits on top of that. And a decade of people talking about their holdings online
sits on top of *that*.

Notice what kind of problem this is. These are **records held by third parties,
which you can neither audit nor revoke.** You cannot un-create a record. You cannot
un-leak a leak. Whatever the exchange knows about you, it knows permanently, and so
does anyone who ever obtains what the exchange knows.

![A KYC record goes into a shredder and comes out intact. You cannot un-leak a leak.](assets/m3-shredder.png)

Which means discretion has a very unusual cost curve, and both halves of it run
against you. The price of staying private compounds with every year you hold and
every counterparty you deal with. The benefit shrinks as the pile of
already-leaked records grows, because your discretion is only worth something if
nobody else has already published you. You are paying more, every year, for
something worth less, every year.

![Two schematic curves: the cost of staying private rising, its value falling. Neither is quantified; the shape is the claim.](assets/m2-scissors.png)

And if you are tax-compliant, the strategy is not even available. Where holdings
or gains are reportable, "leave no record" is not discretion — it is a crime. So
the honest holder is told to hide, by people who have not noticed that hiding is
something the law does not permit them to do.

I have a whole post coming about the French tax-administration case that puts this
beyond argument. For now: the list exists, you are on it, and you were never asked.

## What kind of claim this is

A fair question at this point is: how would you know if this were wrong?

You wouldn't, and I want to be straight about that rather than dress it up.

This is not a prediction you could falsify by counting. It is a claim about
structure — about what people with these incentives, facing these constraints, do.
The cases and the counts in this post are **illustrations of the structure, not
evidence for it**. If the registry showed half as many attacks next year, not one
sentence above would become false; the incentives would be exactly what they are
now.

That sounds like a weakness. There is a longer argument that it isn't — and a much
more uncomfortable argument about why, in this particular field, the evidence that
*would* settle things is systematically unavailable. Both are coming in a later
post. For now I will just flag it, because an argument that quietly relies on data
it cannot produce is doing something dishonest, and I would rather say the thing
out loud.

## The advice was inherited, not derived

So here is the uncomfortable bit.

The standing advice — hold quietly, deny it if asked, keep a small wallet to hand
over — is perfectly sensible advice **for the world of those four conditions.** In
a world where almost nobody is looking for you and nobody can pick you out of a
crowd, staying quiet is close to a complete defence, because the attack mostly
never starts.

That advice was never derived from a threat model. It was inherited from a period.
And the period ended.

What it turns into, once the window closes, is two separate problems that I will
take one at a time.

The first is that it stopped being a mechanism. A defence whose entire strength is
that the attacker does not know something is not something you can rely on once
the attacker knows — and in security engineering, that has a name and a
catalogue entry, and everyone agrees it is a design defect, right up until the
asset in question is bitcoin. That's the next post but one.

The second is worse, and it is the reason I ended up writing papers about this
rather than a checklist. Under the conditions we now actually live in, that advice
does not merely stop protecting people. It **makes their situation worse** — both
during an attack and after one, and not only for the person who followed it. That
one takes more space than a blog post, and it is where the real argument is.

There is no version of this where the window reopens. Every one of the four
conditions is gone in a direction that does not reverse: knowledge doesn't
un-spread, holders don't become rare again, leaked lists don't unleak, and organised
crime doesn't forget a working business model.

The good news, such as it is, is that a defence that never depended on the
attacker's ignorance doesn't care about any of this. Building one turns out to be
possible. It just isn't what anybody is currently telling you to do.

---

*The full arguments are in two open-access papers:*
[***The Deadly Race***](https://doi.org/10.5281/zenodo.22778256) *— what follows
from the fact that you cannot prove you forgot something; and*
[***The Denial Spiral***](https://doi.org/10.5281/zenodo.22778480) *— why advice to
conceal and deny gets worse for everyone the more people take it. Both are free,
neither is behind a signup.*

*Incident data in this post comes from* [*Jameson Lopp's public registry of
physical attacks*](https://github.com/jlopp/physical-bitcoin-attacks)*, which is a
press-sourced sample: it misses everything unreported and over-represents whatever
made the news. New cases I find go upstream to that registry rather than into any
database of mine, because that information belongs to everyone — including whoever
is next.*
