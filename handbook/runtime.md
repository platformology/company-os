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

**What already exists.** The names, and only the names — the full page is **[runtime-brain.md](runtime-brain.md)**, on `main`, and this map does not restate it:

- **Gemma 4 26B 8-bit on this M1** is the shared always-on hand — **after Michael says go**, not before.
- **Llama 3.3 70B 4-bit on this M1** is the on-purpose pen. It is **not a second seat brain.**
- **Flash 2-bit** stays on the M5, SmarterVoice only, and **the M5 is parked**.
- **The M1 is the office.** The M5 is the shop only. Daily Grok Bot lives on this M1.
- **The token rule:** weekday 8am, then 11, 2, and 5. No hourly Grok Bot wakes. The hours between those four windows are exactly the hours a local hand would cover — after go.

**What is still missing.** Michael's go. **"No local LLM" holds until he says go** — that is the lock's own wording on [locks.md](locks.md), and it is a wait, not a forever. What lifting it involves is on that page and in Notion; this map does not restate it, and lifting it is Michael's call, not this map's. Until then the brain is **named, not installed**: nothing here tells anyone to install a model or any other software, and this repo has no install step in it at all.

**Done-check.** You can say out loud which named hand belongs to which machine and what each is for — Gemma 4 26B 8-bit shared and always-on on this M1 after go, Llama 3.3 70B 4-bit as the on-purpose pen rather than a second seat brain, Flash 2-bit on the parked M5 for SmarterVoice only — and you can point at the line in [locks.md](locks.md) that holds all of it until Michael says go. After go, the check becomes: the shared hand runs on this M1 and covers the hours between the token windows, and no seat got a model of its own to make that work.

**Seats are never rebuilt as local models** — that one is on [locks.md](locks.md) and it does not end at go. A seat is a job plus a skill; a hand is something it borrows.

---

## 2. Body / hands — the tools already on this Mac

**What it is.** What the seat can actually touch — read a page, draft a message, file a document, look at a calendar. Instructions with no hands are a reading exercise.

**What already exists.** Five connected tools on this computer, and that is the whole hand:

- Notion
- Gmail
- Calendar
- Slack
- Google Drive

**What is recorded now.** Seat by seat, which of those five a seat touches and what it is denied, is written down on **[runtime-body.md](runtime-body.md)** — on `main`, open it. This map does not copy that table, and whatever is still open about a seat's hands is named on that page in its own words, not summarized here.

**Still true regardless:** **no sixth tool gets added**, and no new CRM — HubSpot is closed and is not a system of record ([clients.md](clients.md)).

**Done-check.** Open one assigned seat's row on [runtime-body.md](runtime-body.md) and name, without guessing, which of the five tools it uses and whether it drafts, files, or only reads — and the list is still five. Then confirm the obvious one: **nothing was sent.** Anything external still stops with Michael ([locks.md](locks.md)).

---

## 3. Wiring / electrical — seats talk to each other without the PA in the middle

**What it is.** One seat's finished work reaching the next seat directly, over a wire that already exists — rather than a person in the middle carrying it, which is what makes work stop when that person is away.

**What already exists.** The wire. Each seat is already a Grok Bot teammate with its own chat, and that chat is the wire — nothing gets installed to carry a handoff. Around it: every seat has a router of its own, listed in [seat-job-map.md](seat-job-map.md), and every job ends at the same gate, [reviews/last-gate-checklist.md](../reviews/last-gate-checklist.md).

**What is recorded now.** Which seat hands its finished work to which owner, and who checks it last, is written down on **[runtime-wiring.md](runtime-wiring.md)** — last-gated, in QC, merging now, so it is the one sister not yet on `main`. Read it there. This map does not copy it, and **nobody invents a sixth tool, a board, or a dashboard** in the meantime.

**Done-check.** Two seats finish one job between them, and you can point at where the first seat's work landed and which seat picked it up — and the PA did not carry it between them. The PA still last-gates before anything external leaves; that is steering, not carrying.

---

## 4. Guts — the seat does the next named job

**What it is.** The seat picking work up and finishing it, rather than sitting still until someone speaks to it.

**What already exists.** How a seat picks up its next named leftover is written down on **[runtime-guts.md](runtime-guts.md)** — on `main`, open it. Underneath it, unchanged: [cheap-loop.md](cheap-loop.md) is how one pass runs, [run-always-on](../skills/run-always-on/SKILL.md) is the cycle it runs inside, and the seat's row in [seat-job-map.md](seat-job-map.md) says which router to open. This map restates none of the four.

**What is still missing.** The named leftovers themselves — for most seats, this repo does not list what is actually left over and waiting behind that seat's job. And **who fills each seat is still unrecorded except COO** (Anthony C. Garcia). Neither gets filled from a guess.

**Done-check.** The seat opens its router, takes the next **named** leftover, last-gates, and stops — and you can name the job it took. That is the whole check. Not "faster." Not "productivity up." No number belongs in it, because nobody measured one.

---

## The four sister pages

Each piece above has its own page, and **all four are written.** Three are on `main` and open the moment you click them. Wiring is the last sister still in QC — a page in QC is a real page waiting on a reviewer, not a page that doesn't exist.

| Piece | Page | Where it is right now |
|---|---|---|
| Brain | [runtime-brain.md](runtime-brain.md) | **On `main`.** Click it. |
| Body / hands | [runtime-body.md](runtime-body.md) | **On `main`.** Click it. |
| Wiring | [runtime-wiring.md](runtime-wiring.md) | Last-gated, in QC, merging now — the last sister not yet on `main` |
| Guts | [runtime-guts.md](runtime-guts.md) | **On `main`.** Click it. |

The wiring link starts working the moment that PR lands. Until then, ask for the open PR — and don't tell anyone the page doesn't exist, because it does.

Each of those pages owns its own detail. This map gives you the one line per piece above and nothing more: it does not restate them, does not summarize them, and does not guess at what they say.

## Seats this page does not build

- **Head of Demand, Head of Sales, and SDR stay unassigned.** No brain, hands, wiring, or guts gets built for a seat nobody is in.
- **Head of Engineering and Developer stay parked.** Building a runtime piece is not unparking a seat.

## Locked, on every one of the four

- **This repo is docs only.** No scripts, no services, and no step on this page that runs a command or installs anything.
- **No send without Michael. No program GitHub. No VMs. No GKE. No local LLM until Michael says go. Seats are never rebuilt as local models. M5 parked. Blue Sky off the LLC books.** Full list, in its own words: [locks.md](locks.md).
- **The M1 is the office; the M5 is the shop only.** Daily Grok Bot does not move off this M1.
- **Nothing gets invented to close a hole above** — no client, no money figure, no person, no price. The humans here are Jhana, Bob, and Anthony C. Garcia; Dave / Lehi Drew (tech) and David McInnis (Cranberry Press) are vendors, not seat holders ([people.md](people.md)).
- **KPI "Current" stays empty**, and no done-check on this page carries a number. The client counts are a separate fact with their date: 1 Alumni (Cornelia Choe, The Leaders Alliance), 67 Past, 0 Current, 0 Prospect on the 18 Aug 2026 extract; Hoffman is a question ([clients.md](clients.md)).

## A named hole stays a named hole

Every "still missing" line above is a real gap, and it is listed once in [SOURCES.md](../SOURCES.md). An unbuilt piece is something to go build or ask Michael about — it is not a blank to fill in with something plausible so the map looks finished.

The reverse is just as strict: **when a sister page fills a hole, the line here changes and its row in [SOURCES.md](../SOURCES.md) goes with it.** A gap that has been closed and is still written up as missing sends the next person looking for nothing, which is the same failure pointed the other way.

## Where this page's shape came from

Two public checklists, adapted: `nicholasswhite/agent-readiness-checklist`, `CHECKLIST.md` — grouped checks that pass only on something you can observe — and `DenisSergeevitch/agents-best-practices`, `references/mvp-agent-blueprint.md` — a numbered build order where the working baseline comes first and the extras come after. The what-exists / what's-missing pair under each piece comes from `petekp/agent-skills`, `skills/autonomous-agent-readiness/SKILL.md`. The sister-page table's "where it is right now" column is the documentation-status rule from `Moonweave-AI/governance`, `05-Knowledge/en/01-Documentation-Guide.md`: a document that doesn't say what state it is in cannot be trusted, and pages in the same repo are linked relatively. Their scores, ratings, and status vocabularies were left behind. Full attribution, with links: [SOURCES.md](../SOURCES.md).
