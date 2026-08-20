# handbook/bodies/ — one file per seat, and the three places a person runs it

A **body** is one seat written out so it can be run: what you are, what you own, what you may touch, how a pass ends. One file, one seat. Pick your seat below, open its body, do the job.

Nothing in this folder needs installing. In Claude and on this Mac a body is a file you open; in the office hand it is the text that goes into one Modelfile, on weights that are already on the machine.

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

## The twenty-three seats Michael named on 20 Aug 2026

All unassigned, all refusing work. Each body says the seat is empty, names what would have to exist first, and stops. Same slugs as [seats/](../seats/README.md) and [desks/](../desks/README.md).

| Seat | Body | Cluster |
|---|---|---|
| Senior Digital Designer | [senior-digital-designer.md](senior-digital-designer.md) | Design, in Craft |
| Junior Digital Designer | [junior-digital-designer.md](junior-digital-designer.md) | Design, in Craft |
| Senior Print and Book Designer | [senior-print-designer.md](senior-print-designer.md) | Design, in Craft |
| Junior Print and Book Designer | [junior-print-designer.md](junior-print-designer.md) | Design, in Craft |
| Social Media Strategist | [social-media-strategist.md](social-media-strategist.md) | Social, under the CMO |
| Social Media Account Expert | [social-account-expert.md](social-account-expert.md) | Social, under the CMO |
| Book Strategist | [book-strategist.md](book-strategist.md) | Book bench, under the CCO |
| Book Writer | [book-writer.md](book-writer.md) | Book bench, under the CCO |
| Book Conceptual Editor | [book-conceptual-editor.md](book-conceptual-editor.md) | Book bench, under the CCO |
| Book Copy Writer | [book-copy-writer.md](book-copy-writer.md) | Book bench, under the CCO |
| Book Technical Editor | [book-technical-editor.md](book-technical-editor.md) | Book bench, under the CCO |
| Book Reader | [book-reader.md](book-reader.md) | Book bench, under the CCO |
| Persona Architect | [persona-architect.md](persona-architect.md) | Craft — not a second COO |
| Strategist | [strategist.md](strategist.md) | Craft |
| Copy Writer | [copy-writer.md](copy-writer.md) | Craft |
| Sales Writer | [sales-writer.md](sales-writer.md) | Craft |
| Copy Editor | [copy-editor.md](copy-editor.md) | Craft |
| Sales Editor | [sales-editor.md](sales-editor.md) | Craft |
| SEO Expert | [seo-expert.md](seo-expert.md) | Growth, under the CMO |
| PR and Media | [pr-media.md](pr-media.md) | Growth, under the CMO |
| University Speaking Booker | [speaking-universities.md](speaking-universities.md) | Stage, under the CMO |
| Association and Corporate Speaking Booker | [speaking-associations.md](speaking-associations.md) | Stage, under the CMO |
| Pendulum Wiki Researcher | [pendulum-wiki.md](pendulum-wiki.md) | Under the Head of Content |

**No seat model gets built for any of them.** The Modelfile recipe below is for the assigned seats; an unassigned seat does not get an alias built so the bench looks staffed. Two places to run these bodies, not three: paste one into Claude, or read it here on this Mac.

Forty-six seats in total, the same forty-six written in [seats/](../seats/README.md). A body adds no seat, no job, and no fact — it is the seat page plus the hands already recorded in [runtime-body.md](../runtime-body.md), written as one runnable file. **If a body and its seat page ever disagree, the seat page wins.**

A body repeats what those two pages already say, and that is on purpose: a model handed nothing but this file cannot follow a link, so the seat has to be complete inside it. The repetition stops at the seat. Prices, clients, people, and the locks are not copied into a body — they stay on the one page that owns each of them.

## The three places you run a body

Same file all three times. You do not rewrite it for the place it is going.

**1. Claude.** Open a new chat, paste or upload the body file, then give it the job. That is the whole setup.

**2. This Mac.** The body is a file on disk in this repo — open it and work off it yourself. This is the version a new hire reads on day one, and it needs no model at all.

**3. The office hand.** Build a seat model whose SYSTEM is that body, on the shared weights already on this M1 — the recipe is below.

## The hand

Recorded 20 Aug 2026 — Michael:

- The local office hand is the Ollama alias **`office-hand`** = **`qwen3.8:27b-q8_0`**, num_ctx **8192**. Daily calls run with thinking off.
- **Gemma 4 31B Q6 stays on disk as backup only.**
- **Do not pull Flash onto this M1.** Do not pull Qwen 16-bit.
- **The M1 is the office**, and Grok Bot stays the manager. Nothing in this folder moves either one.
- **Seats are never rebuilt as local models.** One set of weights, twenty-three bodies. Do not create a weight file per seat, and do not download a second model to give a seat its own.

That last one is a lock, not a preference, and it is the reason this folder exists as markdown instead of as models: what changes per seat is the SYSTEM text, and nothing else.

## The Modelfile — SYSTEM is the only line that changes

Make this on the Mac, next to the model. It is not checked into this repo; this repo is markdown, and the example below is the whole recipe:

```
# ollama create pa -f ./Modelfile.pa
FROM qwen3.8:27b-q8_0
PARAMETER num_ctx 8192
SYSTEM """
...paste the entire contents of handbook/bodies/pa.md here...
"""
```

Then build it and run it:

```
ollama create pa -f ./Modelfile.pa
ollama run pa --think=false "Today's list, off the Do this page."
```

For the next seat, copy that file and change exactly two things: the name after `ollama create`, and the body pasted into `SYSTEM`. **`FROM` never changes** — every seat model points at the same 8-bit weights the office hand already runs, so twenty-three seat models cost one download, not twenty-three. Thinking off is a per-call setting, not a line in the file: `--think=false` on the command, `"think": false` on an API call.

## What a body does not carry, on purpose

A body run in the office hand has no files and no browser. It cannot open [offers.md](../offers.md), [clients.md](../clients.md), or a Notion page, and it does not remember what is on them.

So no body carries a price, a client fact, a person, a KPI, or a stack. When a job needs one of those, the honest answer is **"not in hand — open the page"**, and the person opens it. A remembered price is a wrong price, and a filled-in gap is worse than a blank. **Named missing stays named missing**, in the words the seat page already uses.

## Before anything leaves your hands

- Read [locks.md](../locks.md) first, on the page itself. This folder points at that list and does not keep a copy of it — a second copy drifts, and a drifted lock is a broken one.
- Run [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md) last, every line, honestly.
- **Buyer-facing work gets a human last pass. No send without Michael** — a body drafts, a person sends.

## Leftovers

- [locks.md](../locks.md) and [runtime-brain.md](../runtime-brain.md) were written before the hand above was named, and they still read that way — including which model is the shared one. Both are Michael's to change, not this page's. Flag it to him rather than editing around it, and until he does, the lock page is the one that governs.
- The shapes this folder reused are named in [SOURCES.md](../../SOURCES.md), and the kit URLs stay there. A person running a seat does not need them on this page.
