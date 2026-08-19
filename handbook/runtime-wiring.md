# Runtime wiring — how the seats hand work to each other

This is the electrical system: which seat hands a finished thing to which other seat, on what wire, and who checks it last. It is not a new chat product, not a new tool, and not a new seat. Every seat, reporting line, and skill named below already exists in [seats/](seats/README.md) and [seat-job-map.md](seat-job-map.md).

The map for the whole runtime is `handbook/runtime.md` — in flight, being written now. This page is one part of it: the wiring.

## The wire already exists

Each seat is already a Grok Bot teammate with its own chat, and a chat can be messaged. **That is the wire.** A report hands its finished work to its owner by messaging that seat's chat — the PA is not a relay in the middle of it.

Nothing gets installed to make that work:

- **No Slack as the bot bus.** The seats' own chats are the bus.
- **No Vikunja here.** A desk board after go is Vikunja; go is not this page, and this page does not start it.
- **No home-built dashboard.** A dashboard is a thing to maintain, and nothing on this page needs one.

## Who talks to whom

The report runs the job. The C-suite seat owns the function the job sits inside. The line between them is on the seat pages — this table is the index, not a new org chart.

| Seat that runs the job | Hands the finished thing to | Function that owner is checking |
|---|---|---|
| [Head of Content](seats/head-of-content.md) | [CMO](seats/cmo.md) | Positioning and the public offer ladder staying accurate |
| [Client Success](seats/client-success.md) | [Head of Author Success](seats/head-of-author-success.md) | Author outcomes and the FAQ gate |
| [Head of Author Success](seats/head-of-author-success.md) | [CCO](seats/cco.md) | Author success, campaign QA, retreat experience |
| [Controller](seats/controller.md) | [CFO](seats/cfo.md) | The monthly close inside how money moves |
| [Bookkeeper](seats/bookkeeper.md) | [CFO](seats/cfo.md) | Bills and the general ledger |
| [People Ops](seats/people-ops.md) | [CHRO](seats/chro.md) | Who's on the roster and how they're classified |
| [Campaign Coordinator](seats/campaign-coordinator.md) | [CCO](seats/cco.md) **and** [VP Campaigns](seats/vp-campaigns.md) | CCO: campaign QA on the live campaign. VP Campaigns: the Campaign SOP the coordinator ran |
| [Retreat Producer](seats/retreat-producer.md) | [VP Retreats](seats/vp-retreats.md) | The Retreat and PIAB SOPs |
| Any seat, when the finished thing is a Company OS / docs change | [COO](seats/coo.md), then [PA](seats/pa.md) | First QC on the docs, then the last gate |

**The [Campaign Coordinator](seats/campaign-coordinator.md) has two owners, and both are named on purpose.** The seat reports into CCO and VP Campaigns. Two owners is not two stamps: each one checks the function it actually owns — campaign QA is the [CCO](seats/cco.md)'s, the Campaign SOP is [VP Campaigns](seats/vp-campaigns.md)' — and neither signs off on the other's half. Don't collapse the Coordinator into VP Campaigns to make the row shorter, and don't hand the CCO's half to the [CMO](seats/cmo.md), who does not own campaign day-to-day at all. Both lines are already on the seat pages: [seats/campaign-coordinator.md](seats/campaign-coordinator.md) records the seat reporting to CCO and VP Campaigns, [seats/cco.md](seats/cco.md) records the Coordinator reporting into it, and the roster row in [seats/README.md](seats/README.md) reads the same way.

Three groups are not on this table, and no wire is run to them:

- **[Head of Demand](seats/head-of-demand.md), [Head of Sales](seats/head-of-sales.md), [SDR](seats/sdr.md) stay unassigned.** No live work is handed to them, and nothing here gives them a queue.
- **[Head of Engineering](seats/head-of-engineering.md) and [Developer](seats/developer.md) are parked.** No wire on this page starts code.
- **A seat whose page records no line above it** has a named-missing hole, not a line to guess. Read the seat page; if it doesn't say, that's the answer.

## Three layers, in this order

Michael's word, 19 Aug 2026:

1. **The employee seat QCs the skill it ran.** Its own row in [seat-job-map.md](seat-job-map.md), its own output.
2. **The C-suite seat QCs the function it owns** — the column above, and nothing wider. Where the table names two owners, each one runs this layer on its own half.
3. **The [COO](seats/coo.md) is first QC on the Company OS and on docs PRs** — first, not only. See [run-coo](../skills/run-coo/SKILL.md).
4. **The [PA](seats/pa.md) last-gates, then merges** a docs PR — after the gate passed and the COO's first QC happened. See [run-pa](../skills/run-pa/SKILL.md) and [last-gate-then-stop](../skills/last-gate-then-stop/SKILL.md).

Three rules hold across all four:

- **Silent to Michael on routine QC.** A pass produces no ping. Michael hears about it when a QC failure blocks a sourced slice, or when the item is already on the ask-Michael-first list in [locks.md](locks.md).
- **Crossed-seat sign-off is a miss, not a pass.** A seat signing off on a function it does not own has not QC'd anything — it has added a stamp. One layer per step, no stamp on top of a stamp.
- **Do not fan a skill to seats that do not own it.** One skill, the seat whose row it is on, one report at a time. See [run-always-on](../skills/run-always-on/SKILL.md).

## What the PA is on this wire

The PA **communicates, connects, reviews, and optimizes.** It is not the workhorse, and every employee seat has to run its own job on this computer without the PA writing that job for it.

So on this wire the PA is exactly two things:

- **The last gate**, running [reviews/last-gate-checklist.md](../reviews/last-gate-checklist.md) on what arrives, then merging the docs PR or handing the thing to Michael.
- **The assigner of the next leftover**, one at a time, when a seat's named queue runs out and the next unit of work sits outside that seat's own row.

And it is not:

- **Not the writer.** A page the PA wrote is a page no seat produced.
- **Not the QC of a skill it does not own.** That is the crossed-seat miss above, and the PA is not an exception to it.
- **Not the middle of every handoff.** Report to owner is a direct message, seat to seat.

## When a seat is blocked

Name it and stop. In the message to the owner seat — both owners, where its row names two — the blocked seat writes one of two things:

- **The lock** that stops it, quoted from [locks.md](locks.md) — no send without Michael, no program GitHub, no VMs, no GKE, no local LLM, M5 parked, Blue Sky off the LLC books.
- **The named-missing hole**, quoted from the list in [SOURCES.md](../SOURCES.md), in the words that list already uses.

Then it stops. It does not ping Michael, and it does not route around the lock. If the block is an ask-Michael-first item, it travels this same wire up to the PA — the seat that hands things to Michael — and the blocked seat still does not message Michael itself.

A block is not permission to invent work. An empty queue is a failure, and the answer to it is in [cheap-loop.md](cheap-loop.md): learn or improve the same named job from a gap already named in [SOURCES.md](../SOURCES.md). Never a new job, a new client, a new offer, or a new number.

## When the seats talk

Weekday **8am, then 11, 2, and 5** — Michael's word, 19 Aug 2026. **No hourly Grok Bot wakes.** A handoff message sits in the owner seat's chat until its next window; that wait is the design, not a delay to work around.

This is a wake cadence for bot seats, not a meeting. The meeting cadence is the four rows in [run-meetings](../skills/run-meetings/SKILL.md), and this page adds no slot to it. Off-hours silence from a human is silence — not approval, and not a reason to proceed.

## Done-check: one finished page, start to finish

A new hire can follow this without the PA writing a word of it:

1. A report opens its row in [seat-job-map.md](seat-job-map.md), runs the skill through [cheap-loop.md](cheap-loop.md), and finishes the page.
2. It QCs the skill it just ran — layer one.
3. It messages its owner's chat from the table above — both owners' chats, if its row names two — and stops.
4. Each owner QCs the function it owns — layer two — and says pass or names the miss.
5. It's a docs change, so the [COO](seats/coo.md) first-QCs it. No ping to Michael either way.
6. The [PA](seats/pa.md) runs the last gate, then merges. If the gate fails, the PA names the unchecked line and does not soften it.

Every hand on that page belonged to the seat that owned the work. The PA gated it and merged it.

## Where these facts come from

The seats, the reporting lines, and the routers are already recorded in [seats/](seats/README.md) and [seat-job-map.md](seat-job-map.md). The locks are [locks.md](locks.md), the loop is [cheap-loop.md](cheap-loop.md), the cycle is [run-always-on](../skills/run-always-on/SKILL.md), and the gate is [reviews/last-gate-checklist.md](../reviews/last-gate-checklist.md). The three QC layers and the 8am / 11 / 2 / 5 windows are Michael's word on 19 Aug 2026. Nothing else on this page is new.

## Never

- Never put the PA in the middle of a report-to-owner handoff, and never let the PA write the work it is going to gate.
- Never sign off on a function your seat does not own, and never add a second stamp to something already QC'd.
- Never drop one of a seat's two owners to make a row shorter — the Campaign Coordinator answers to both the CCO and VP Campaigns.
- Never hand live work to Demand, Sales, or SDR, and never start code from the parked engineering seats.
- Never install a bus, a board, or a dashboard to make this wiring work — the seats' own chats are the wire.
- Never ping Michael to report a routine QC pass, and never ping him instead of naming the lock or the hole.
- Never wake a seat hourly.
- Never send anything without Michael. No program GitHub. See [locks.md](locks.md).
