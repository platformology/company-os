# Runtime — the four pieces that make a bot seat work like a person

Recorded 19 Aug 2026 — Michael. **The pages and skills in this repo are the instructions, not the person.** A seat with a good job description still does not work like a person until four pieces are built underneath it. This page is the build map for those four, in order: **brain, hands, wiring, guts** — every assigned bot seat functions like a person on this Mac, and *then* we write the growth plans.

This is a build map. It is not a seat router — [seat-job-map.md](seat-job-map.md) already does that job — and it is not a plan for the business.

## Read this once, in order

1. **Brain** — a local model, a local hand on this Mac.
2. **Body / hands** — the tools already on this Mac.
3. **Wiring / electrical** — seats talk to each other without the PA in the middle.
4. **Guts** — the seat does the next named job.

Build one, two, three, four. Nothing later on the list gets built first because it sounds easier. Each of the four has its own page — the four links are at the bottom of this map.

**Later, and not on this page:** business plans, marketing plans, R&D plans, timelines, sprints. Those come after these four are built. Do not write them here, and do not let a missing plan become the reason a piece above stays unbuilt.

## Who does what while these get built

The PA steers and last-gates. Claude / Other Models writes the heavy pages. Grok seats QC. The seat does the job. **The PA is not the workhorse** — a piece of this build that only moves when the PA personally moves it is not built.

---

## 1. Brain — a local model, a local hand on this Mac

**What it is.** Where the seat's thinking happens. Today a seat only thinks inside its scheduled windows; a brain on this machine is what would let it think in the hours between them.

**What already exists.** The names, and only the names:

- **Gemma on the M1** is the one hand — **after Michael says go**, not before.
- **Flash on the M5** is one hand for SmarterVoice only, and **the M5 is parked**.
- **The M1 is the office.** The M5 is the shop only. Daily Grok Bot lives on this M1.
- **The token rule:** weekday 8am, then 11, 2, and 5. No hourly Grok Bot wakes. The hours between those four windows are exactly the hours a local hand would cover — after go.

**What is still missing.** Michael's go. **"No local LLM" is still a lock** — see [locks.md](locks.md). The brain is **named, not installed**: nothing on this page tells anyone to install a model, or any other software, and this repo has no install step in it at all. Also missing: which named hand belongs to which assigned seat. Not recorded, not guessed.

**Done-check.** You can say out loud which named hand belongs to which machine and what it is allowed to do — Gemma on the M1 after go, Flash on the M5 for SmarterVoice only, the M5 parked — and you can point at the line in [locks.md](locks.md) that keeps a local model off this machine until then. After Michael says go, the check becomes: the named hand runs on the M1 and covers the hours between the token windows, and no second model was added to make that work.

**Do not** rebuild a seat as a local model. A seat is a seat; a brain is one hand it gets to use.

---

## 2. Body / hands — the tools already on this Mac

**What it is.** What the seat can actually touch — read a page, draft a message, file a document, look at a calendar. Instructions with no hands are a reading exercise.

**What already exists.** Five connected tools on this computer, and that is the whole hand:

- Notion
- Gmail
- Calendar
- Slack
- Google Drive

**What is still missing.** Seat by seat, which of those five a seat touches for its named job, and what it is allowed to do with each — draft, file, or read only. Not recorded. **No sixth tool gets added to close that gap**, and no new CRM: HubSpot is closed and is not a system of record ([clients.md](clients.md)).

**Done-check.** Open one assigned seat's job and name, without guessing, which of the five tools it uses and whether it drafts, files, or only reads — and the list is still five. Then confirm the obvious one: **nothing was sent.** Anything external still stops with Michael ([locks.md](locks.md)).

---

## 3. Wiring / electrical — seats talk to each other without the PA in the middle

**What it is.** One seat's finished work reaching the next seat directly. Today anything crossing between two seats crosses through a person, which means work stops when that person is away.

**What already exists.** The two things that make a handoff legible: every seat has a router of its own, listed in [seat-job-map.md](seat-job-map.md), and every job ends at the same gate, [reviews/last-gate-checklist.md](../reviews/last-gate-checklist.md). So a seat already knows what it runs and where it stops.

**What is still missing.** The path itself. Which of the five connected tools carries a handoff from one seat to the next, where it lands, and how the receiving seat knows it arrived — none of that is recorded here. It stays named missing until Michael sources it. Nobody invents a queue, a board, or a message format to fill it.

**Done-check.** Two seats finish one job between them, and you can point at where the first seat's work landed and which seat picked it up — and the PA did not carry it between them. The PA still last-gates before anything external leaves; that is steering, not carrying.

---

## 4. Guts — the seat does the next named job

**What it is.** The seat picking work up and finishing it, rather than sitting still until someone speaks to it.

**What already exists.** The loop and the cycle are already written: [cheap-loop.md](cheap-loop.md) is how one pass runs, [run-always-on](../skills/run-always-on/SKILL.md) is the cycle it runs inside, and the seat's row in [seat-job-map.md](seat-job-map.md) says which router to open. This page does not restate any of the three.

**What is still missing.** The named leftovers themselves — for most seats, this repo does not list what is actually left over and waiting behind that seat's job. And **who fills each seat is still unrecorded except COO** (Anthony C. Garcia). Neither gets filled from a guess.

**Done-check.** The seat opens its router, takes the next **named** leftover, last-gates, and stops — and you can name the job it took. That is the whole check. Not "faster." Not "productivity up." No number belongs in it, because nobody measured one.

---

## The four sister pages

Each piece above has its own page, and **all four are written** — each one is in QC on its own sister PR, so it is not on this branch yet. Go read the page for the piece you are building:

- [runtime-brain.md](runtime-brain.md) — the brain: a local model, a local hand on this Mac.
- [runtime-body.md](runtime-body.md) — the hands: the tools already on this Mac.
- [runtime-wiring.md](runtime-wiring.md) — the wiring: seats talk to each other without the PA in the middle.
- [runtime-guts.md](runtime-guts.md) — the guts: the seat does the next named job.

Those four links resolve once the sister PRs land. Until then the page is in QC, not missing — ask for the open PR rather than assuming there is nothing to read.

Each of those pages owns its own detail. This map gives you the one line above and nothing more: it does not restate them, does not describe them in advance, and does not guess at what they say.

## Seats this page does not build

- **Head of Demand, Head of Sales, and SDR stay unassigned.** No brain, hands, wiring, or guts gets built for a seat nobody is in.
- **Head of Engineering and Developer stay parked.** Building a runtime piece is not unparking a seat.

## Locked, on every one of the four

- **This repo is docs only.** No scripts, no services, and no step on this page that runs a command or installs anything.
- **No send without Michael. No program GitHub. No VMs. No GKE. No local LLM. M5 parked. Blue Sky off the LLC books.** Full list: [locks.md](locks.md).
- **The M1 is the office; the M5 is the shop only.** Daily Grok Bot does not move off this M1.
- **Nothing gets invented to close a hole above** — no client, no money figure, no person, no price. The humans here are Jhana, Bob, and Anthony C. Garcia; Dave / Lehi Drew (tech) and David McInnis (Cranberry Press) are vendors, not seat holders ([people.md](people.md)).
- **KPI "Current" stays empty**, and no done-check on this page carries a number. The client counts are a separate fact with their date: 1 Alumni (Cornelia Choe, The Leaders Alliance), 67 Past, 0 Current, 0 Prospect on the 18 Aug 2026 extract; Hoffman is a question ([clients.md](clients.md)).

## A named hole stays a named hole

Every "still missing" line above is a real gap, and it is listed once in [SOURCES.md](../SOURCES.md). An unbuilt piece is something to go build or ask Michael about — it is not a blank to fill in with something plausible so the map looks finished.

## Where this page's shape came from

Two public checklists, adapted: `nicholasswhite/agent-readiness-checklist`, `CHECKLIST.md` — grouped checks that pass only on something you can observe — and `DenisSergeevitch/agents-best-practices`, `references/mvp-agent-blueprint.md` — a numbered build order where the working baseline comes first and the extras come after. The what-exists / what's-missing pair under each piece comes from `petekp/agent-skills`, `skills/autonomous-agent-readiness/SKILL.md`. Their scores and ratings were left behind. Full attribution, with links: [SOURCES.md](../SOURCES.md).
