# handbook/bodies/ — one file per seat, and the three places a person runs it

A **body** is one seat written out so it can be run: what you are, what you own, what you may touch, how a pass ends. One file, one seat. Pick your seat below, open its body, do the job.

Nothing in this folder gets installed. Two of the three places below work today, because a body is a file you open — and on this Mac it needs no model at all. The third, the shared office hand, is **named and not on this machine**: it waits on Michael's go, and no step on this page puts it there.

**Two "body"s, one word.** [runtime-body.md](../runtime-body.md) is about *hands* — which of the five connected tools a seat may touch. A **body file** in this folder is the seat itself, written so a person or a model can run it. Don't read one as the other.

## Pick your seat

| Seat | Body | Status |
|---|---|---|
| PA | [pa.md](pa.md) | Assigned |
| COO | [coo.md](coo.md) | Assigned |
| CMO | [cmo.md](cmo.md) | Assigned |
| Head of Content | [head-of-content.md](head-of-content.md) | Assigned |
| Head of Demand | [head-of-demand.md](head-of-demand.md) | **Unassigned** — the body says so and refuses work |
| CSO | [cso.md](cso.md) | Assigned |
| Head of Sales | [head-of-sales.md](head-of-sales.md) | **Unassigned** — the body says so and refuses work |
| SDR | [sdr.md](sdr.md) | **Unassigned** — the body says so and refuses work |
| CFO | [cfo.md](cfo.md) | Assigned |
| Controller | [controller.md](controller.md) | Assigned |
| Bookkeeper | [bookkeeper.md](bookkeeper.md) | Assigned |
| CTO | [cto.md](cto.md) | Assigned |
| Head of Engineering | [head-of-engineering.md](head-of-engineering.md) | **Parked** — the body answers about the seat and starts nothing |
| Developer | [developer.md](developer.md) | **Parked** — the body answers about the seat and starts nothing |
| CCO | [cco.md](cco.md) | Assigned |
| Head of Author Success | [head-of-author-success.md](head-of-author-success.md) | Assigned |
| Client Success | [client-success.md](client-success.md) | Assigned |
| CHRO | [chro.md](chro.md) | Assigned |
| People Ops | [people-ops.md](people-ops.md) | Assigned |
| VP Campaigns | [vp-campaigns.md](vp-campaigns.md) | Assigned |
| Campaign Coordinator | [campaign-coordinator.md](campaign-coordinator.md) | Assigned |
| VP Retreats | [vp-retreats.md](vp-retreats.md) | Assigned |
| Retreat Producer | [retreat-producer.md](retreat-producer.md) | Assigned |

Twenty-three seats, the same twenty-three already written in [seats/](../seats/README.md). A body adds no seat, no job, and no fact — it is the seat page plus the hands already recorded in [runtime-body.md](../runtime-body.md), written as one runnable file. **If a body and its seat page ever disagree, the seat page wins.**

A body repeats what those two pages already say, and that is on purpose: a model handed nothing but this file cannot follow a link, so the seat has to be complete inside it. The repetition stops at the seat. Prices, clients, people, and the locks are not copied into a body — they stay on the one page that owns each of them.

## The three places you run a body

Same file all three times. You do not rewrite it for the place it is going.

**1. Claude.** Open a new chat, paste or upload the body file, then give it the job. That is the whole setup.

**2. This Mac.** The body is a file on disk in this repo — open it and work off it yourself. This is the version a new hire reads on day one, and it needs no model at all.

**3. The office hand — after Michael says go, not before.** The shared hand is named and is not on the machine. After go, a seat model's SYSTEM is its body file and nothing else about the seat changes. The shape is below; nothing here installs it.

## The hand — named, not installed

The hand is named on [runtime.md](../runtime.md) and [runtime-brain.md](../runtime-brain.md) — recorded 19 Aug 2026 via the CTO, restated 20 Aug on the build map. This page repeats only the three lines a body needs; those two pages own the rest and this one does not restate them.

- **Gemma 4 26B 8-bit on this M1** is the shared always-on hand — **after Michael says go**, not before. That is the one a body would run on.
- **Llama 3.3 70B 4-bit on this M1** is the on-purpose pen. It is **not a second seat brain**, and no seat gets a body built on it.
- **Flash 2-bit** is the M5, SmarterVoice only, and **the M5 is parked**. No body goes near it.

**Status today: not installed.** **"No local LLM until Michael says go"** is the lock's own wording on [locks.md](../locks.md), and Phase 4 of the go packet is the only thing that lifts it. So there is no local model on this machine, this page tells nobody to put one there, and a page that treats the hand as already running is a broken lock — not a shortcut. Read [runtime-brain.md](../runtime-brain.md) if that is the question you arrived with; the answer there is the same, and it is "don't."

**Seats are never rebuilt as local models.** That one does not lift at go: one shared hand, twenty-three bodies. No weight file per seat, and no second model downloaded so a seat can have its own. It is a lock, not a preference, and it is why this folder is markdown instead of models — what changes per seat is the SYSTEM text, and nothing else.

**The M1 is the office**, and Daily Grok Bot lives on it. Nothing in this folder moves either one, before go or after it.

## After go: SYSTEM is the only thing that changes per seat

Written down so nobody has to re-derive it, and **not a step to take**. What actually gets installed, in what order, and by whom belongs to the go packet behind Phase 4 on [locks.md](../locks.md) — this page does not restate that list and does not start a piece of it early.

The shape is one model definition per seat, every one of them pointing at the same shared weights:

| Part of the definition | What it holds | Changes per seat? |
|---|---|---|
| The base it starts from | the one shared hand named above | **Never.** |
| Its SYSTEM text | the entire contents of that seat's body file | **Yes — this is the only thing.** |
| The name it is built under | the seat, e.g. `pa` | Yes |

Twenty-three seat models, one set of weights. The base never changing is what makes that true, and it is the same lock as "seats are never rebuilt as local models" read from the other end.

Two things this section deliberately does not carry. **No command** — a build or run line written out today is Phase 4 taken early, which is the exact broken lock this page exists to avoid. And **no model tag, context size, or sampler setting**: those are **not recorded in this repo**, they belong to the go packet, and a guessed tag is a wrong tag.

## What a body does not carry, on purpose

A body handed to a model and nothing else — which is what the office hand would be, after go — has no files and no browser. It cannot open [offers.md](../offers.md), [clients.md](../clients.md), or a Notion page, and it does not remember what is on them.

So no body carries a price, a client fact, a person, a KPI, or a stack. When a job needs one of those, the honest answer is **"not in hand — open the page"**, and the person opens it. A remembered price is a wrong price, and a filled-in gap is worse than a blank. **Named missing stays named missing**, in the words the seat page already uses.

## Before anything leaves your hands

- Read [locks.md](../locks.md) first, on the page itself. This folder points at that list and does not keep a copy of it — a second copy drifts, and a drifted lock is a broken one.
- Run [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md) last, every line, honestly.
- **Buyer-facing work gets a human last pass. No send without Michael** — a body drafts, a person sends.

## Leftovers

- **How the hand is actually loaded is not recorded here** — no model tag, no context size, no call settings. That is the go packet's, behind Phase 4 on [locks.md](../locks.md), and it stays named missing in [SOURCES.md](../../SOURCES.md) rather than guessed at on this page.
- **Lifting the lock is Michael's, and so is changing it.** If a seat needs the hand before he says go, the answer is the lock and a stop — not a smaller version of the install. Run [check-locks](../../skills/check-locks/SKILL.md), name the lock, stop.
- The shapes this folder reused are named in [SOURCES.md](../../SOURCES.md), and the kit URLs stay there. A person running a seat does not need them on this page.
