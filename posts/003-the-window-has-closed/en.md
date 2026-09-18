
# The Window Has Closed

Everyone gives the same advice about not getting robbed for your bitcoin. Don't
tell anyone. If someone asks, deny it. Keep a small wallet you can hand over.

I don't think it's stupid advice. I think it was good advice for a world that
stopped existing, and nobody went back to check.

<p align="center"><img src="assets/m1-four-panes.png" alt="The four conditions that made early holding safe, with identification struck out. A claim about incentives, not a measurement." width="460"></p>

## Four things that used to be true

1. Most thieves had never even heard of bitcoin.

2. The ones who had were unlikely to meet you (akin to finding a needle in a haystack).

3. If they did, more likely than not, they wouldn't know that you, specifically,
were a holder. (The window of effectiveness of discretion as a defence.)

4. Finally, if all of that failed and someone did turn up at your door, you probably knew
more than he did. The early holder was typically an OG, cypherpunk or a cryptographer,
someone who'd read the mailing list. The attacker was typically improvising. The
technical asymmetry tended to run your way.

Four separate things, all pointing the same direction. It really was fairly safe
in there.

## None of them hold now

The first two don't need arguing.

The fourth has gone into reverse. French prosecutors have charged 88 people across
a dozen linked kidnapping and extortion cases. That isn't a run of opportunists,
it's organisations, with reconnaissance and division of labour and repeat
business. Meanwhile the holder they're coming for is now, statistically, somebody
who bought some bitcoin on an app. The cryptographer-versus-amateur matchup has
roughly swapped ends.

You can see it in the shape of the attacks too. One industry count for the first
half of 2026 has reported home invasions going from 1 to 20 out of 52 incidents,
year on year. It's moving to where people live.

<p align="center"><img src="assets/m6-home-invasions.png" alt="Reported home invasions rose from 1 to 20 of 52 incidents year on year. Industry count; verified incidents only, press-sourced, directional." width="460"></p>

On counts in general: several series exist, they disagree with each other about
the numbers, and they agree completely about the direction. A handful a year
before 2017, dozens a year now. The registries are built from press reports, so
they miss anything unreported and over-weight whatever made the news. Pick
whichever series you like. They all slope the same way.

That leaves the third condition, which is the one that actually closed the window,
and it needs its own section.

## Somebody has a list — factor 3

To come after you specifically, a thief needs a list. For most of bitcoin's
history there wasn't one.

Now there are several, and you didn't agree to any of them.
Threat-intelligence reporting on the 2026 wave puts victim selection down to
leaked databases, tax records and exchange data, plus insider sales of customer
lists and dark-web recruitment of staff with database access. Chain analysis on
top of that. A decade of people posting about their stack on top of that.

These are records held by other people, which you can't audit and can't revoke.
You can't un-create a record and you can't un-leak a leak. Whatever your exchange
knew about you in 2019 it knows permanently, and so does anybody who has since got
hold of what it knew.

<p align="center"><img src="assets/m3-shredder.png" alt="A KYC record goes into a shredder and comes out intact. You cannot un-leak a leak." width="460"></p>

That does something strange to the economics of keeping quiet, and both halves of
it work against you. Staying private costs more every year: every year you hold,
every counterparty you deal with, every service that suddenly wants a document.
And it's worth less every year, because your discretion only buys you anything if
nobody has published you already.

<p align="center"><img src="assets/m2-scissors.png" alt="Two schematic curves: the cost of staying private rising, its value falling. Neither is quantified; the shape is the claim." width="680"></p>

If you declare your taxes it's worse than that, because the strategy isn't
available to you at all. Where gains are reportable, "leave no record" isn't
discretion, it's a crime. So the honest holder gets told to hide by people who
haven't noticed that the law doesn't let him.

There's a French case coming in the next post that makes this concrete. For now:
the list exists, you're on it, nobody asked you.

## The advice was inherited, not derived

Go back to the counsel. Hold quietly, deny it, keep something to hand over. In a
world where almost nobody is looking for you and nobody can pick you out of a
crowd, that's close to a complete defence, because the attack mostly never starts.

Nobody derived it from a threat model. It got inherited from a period, and the
period ended.

What it turns into afterwards is two separate problems, and I'll take them one at
a time in later posts.

First, it stopped being a mechanism. A defence whose whole strength is the
attacker not knowing something isn't a defence you can lean on once he knows.
Security engineering has a name for that and a catalogue entry, and everybody
agrees it's a design defect right up until the asset in question is bitcoin.

Second, and this is the worse one, and it's why I ended up writing papers instead
of a checklist: under the conditions we actually live in, that advice doesn't
merely stop protecting people. It makes things worse for them, during an attack
and after one, and not only for the person who took it.

None of the four conditions is coming back, either. Knowledge doesn't un-spread,
holders don't get rare again, leaked lists stay leaked, and organised crime
doesn't forget a business model that works.

A defence that never relied on the attacker's ignorance doesn't care about any of
this. Building one turns out to be possible. It just isn't what anybody is telling
you to do.

---

*The full arguments are in two open-access papers:*
[***The Deadly Race***](https://doi.org/10.5281/zenodo.22778256) *— what follows
from the fact that you can't prove you forgot something; and*
[***The Denial Spiral***](https://doi.org/10.5281/zenodo.22778480) *— why advice to
conceal and deny gets worse for everybody the more people take it. Both free,
neither behind a signup.*

*Incident data comes from* [*Jameson Lopp's public registry of physical
attacks*](https://github.com/jlopp/physical-bitcoin-attacks)*, a press-sourced
sample: it misses everything unreported and over-weights whatever made the news.
New cases I find go upstream to that registry rather than into any database of
mine, because that information belongs to everyone, including whoever's next.*

---

**If this was worth your time.** Send it to someone still running the old advice,
that does more than anything else here. A ⭐ on [Great Wall](https://github.com/Yuri-SVB/Great-Wallet),
[the research](https://github.com/Yuri-SVB/great-wall-docs) or [these posts](https://github.com/Yuri-SVB/great-wall-posts)
costs nothing and makes the work easier to find. And if you want to fund it,
[support](https://github.com/Yuri-SVB/support) takes ⚡ Lightning and on-chain, no
signup, no tiers, nothing expected back.
