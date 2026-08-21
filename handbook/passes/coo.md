# COO — one pass, worked

**Status: Assigned** · **Holder: Anthony C. Garcia (public title: COO / Chief Persona Architect)** · **Written: 21 Aug 2026**

[plans/coo.md](../plans/coo.md) is the plan for this seat: what to open, the one job, the SOP behind it, the KPIs it is pointed at. This page is that same pass walked through — where you sit, what you read at each stop, what you write down, and what you leave behind so the next person can pick it up cold without asking you anything.

Read the plan first. This page does not restate it, and it does not restate the seat either: [seats/coo.md](../seats/coo.md) is what the COO owns, [desks/coo.md](../desks/coo.md) is the sit-down pack, [bodies/coo.md](../bodies/coo.md) is the seat as one runnable file, and [run-coo](../../skills/run-coo/SKILL.md) is the router. **If this page and the seat page disagree, the seat page wins, and this page is the thing that gets fixed.**

**Who fills this seat: Anthony C. Garcia.** [people.md](../people.md) records him once, in one row — "Anthony C. Garcia | COO / Chief Persona Architect (public title)" — and that is the whole of what is written down. This is the one seat in the company with a recorded holder, so do not read the blank holder line on the other pass pages onto this one, and do not put a second name beside his. The **Persona Architect** leftover-file plan is a separate seat and **not a second COO** ([SOURCES.md](../../SOURCES.md)). Jhana and Bob have **no Role recorded** ([people.md](../people.md)) — neither of them is in this seat or any other.

**One change, one verdict.** Not two changes, and not a second verdict on something another seat already QC'd.

**Your QC is first, and it is not the last.** The [PA](../seats/pa.md) runs [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md) after you and merges. **You do not last-gate and you do not merge.**

## What you need open

[locks.md](../locks.md), [seats/coo.md](../seats/coo.md), [desks/coo.md](../desks/coo.md), [plans/coo.md](../plans/coo.md), [runtime-wiring.md](../runtime-wiring.md) for the three QC layers, and [run-coo](../../skills/run-coo/SKILL.md) as the router. In Notion: [Grok Bot staff](https://app.notion.com/p/3c125e30d68b81dc9116e2e62b47f143), [Company OS home](https://app.notion.com/p/3c025e30d68b81cdbad7fdf5912e3ca3), [Buyer data room](https://app.notion.com/p/3c025e30d68b8135bdcdc9010e649855), [Do this](https://app.notion.com/p/3c025e30d68b8142a971ccdb0d657b22), and [PA handoff](https://app.notion.com/p/3c125e30d68b8138a686fd8a52313333). Google Calendar: **read the meetings that already exist.** That list is the whole set — do not invent a sixth page, and a tool outside it is a stop rather than an improvisation.

**Do this** and **Buyer data room** are hands, not extra jobs. **Creating a meeting to fill a phase is denied** ([runtime-body.md](../runtime-body.md)), and the calendar is not an hours record — reading a delivery share off it would be inventing the denominator.

## What this seat records, and what it does not

Read this before you go looking for a COO accountability list, because there isn't one here and that is the honest state.

The seat page records **the public title and nothing wider** — "detailed COO accountabilities beyond the public title" is named missing, and **there is no COO SOP recorded in this repo** either ([SOURCES.md](../../SOURCES.md)). The Notion pages above are the fuller picture. Do not draft an SOP from a template to close that gap, and do not borrow another seat's SOP to stand in for one.

Two things still reach you, and both come off the pages that record how this Mac runs rather than off the seat page: **first QC on the Company OS and on docs pull requests**, from [runtime-wiring.md](../runtime-wiring.md), and **one pass of plan, meetings, execution, QC**, from this seat's row on [runtime-body.md](../runtime-body.md). That second one is a finish line written beside the seat's hands, not an accountability the seat page recorded, and it does not get promoted into one here. **This page walks the first QC**, because that is the layer that is written down.

There is also no queue. Nothing in this repo lists docs changes waiting on QC — a change arrives from the seat that produced it, in that seat's own message. **If nothing arrived, nothing arrived**: that is a real answer, and it is not permission to go write a page so you have something to check.

## The pass

**1. Read the change against the locks, first, before anything else.** Open [locks.md](../locks.md) and read the actual change in front of you against it — not the seat in general. **A change that breaks a lock fails QC on that line alone**, and you quote the lock rather than softening it. This step is first on purpose: if the change should not have been made at all, say so now, in one plain sentence, instead of fact-checking a page that is going to be thrown out anyway.

The ones that bite most often here: **"No send without Michael"** — the COO seat is not an exception. **"No program GitHub"** — nothing against `smarter-voice`, `academic-research-platform`, `book-campaign-platform`, `styleguide-os`, `persona-standalone-programs`, or `tlpF-b01-research-engine`. **"Blue Sky stays off the LLC books."** And the machine locks: no VMs, no GKE, no local LLM until Michael says go — and **Qwen is not on the Phase 4 list** — the M1 is the office, and the M5 is the shop and stays parked. A change that writes a run line, a model tag, or the office onto the M5 fails there. The four phases behind them were recorded 19 Aug 2026 — Michael, via the CTO. **The [CTO](../seats/cto.md) seat holds those machine locks and names the one that blocks an ask; it does not lift any of them, and who fills it is not recorded.** Neither fact makes a lock softer.

**2. Check the seat that produced it owned the work.** Find its row in [seat-job-map.md](../seat-job-map.md) and the owner column in [runtime-wiring.md](../runtime-wiring.md). A page produced by a seat that does not own it is a **miss, not a pass** — and so is a page the PA wrote, since the PA then gates its own work. **Head of Demand, Head of Sales, and SDR are unassigned**, and [Head of Engineering](../seats/head-of-engineering.md) and [Developer](../seats/developer.md) are parked, so a change carrying live work for any of those five is a miss on this line.

**3. Check every fact against the page that sources it.** The company first: **Platformology LLC is one company**, and **Promote a Book** and **Book Retreat** are DBAs of it — not two companies, and not SmarterVoice. Then:

- **Prices → [offers.md](../offers.md).** Both numbers where the ladder shows two. **Platinum Major List has no public price.** A change that picked one number, averaged two, or quoted a rung that is not on the ladder fails. **How an Uncovery is sold is named missing** — a change that calls it paid discovery or paid diagnosis has filled in a gap, and that is a miss.
- **Clients → [clients.md](../clients.md)**, with the 18 Aug 2026 extract date attached. **A folder name is not a client. HubSpot is closed. Hoffman is a question, not a Current client. Cornelia Choe is Alumni**, and her two Zoom URLs are still unpicked.
- **People → [people.md](../people.md).** **Jhana and Bob have no Role recorded.** Dave / Lehi Drew and David McInnis are **vendors, not employees**. Who fills the PA seat stays **not recorded**, and who fills the CTO seat stays **missing** — a change that fills either one in is a miss even if the name is plausible.
- **KPI names → the board, and the Current field stays empty.** This seat's two are **Founder delivery hours %** and **Retreat fill rate**, names only. **No figure goes in a Current field — not a percentage, not a headcount, not a 0. A 0 is a figure.** No hours are recorded for anyone, and no next retreat is recorded, so neither of those is something to calculate. Names get quoted whole: the VP Retreats KPI is **"Platform in a Box cycle time"** on the board, and a change that shortens it is a miss on the name. The shortening already sitting on [plans/README.md](../plans/README.md) is named in [SOURCES.md](../../SOURCES.md) — **QC-ing one change is not permission to go edit that index.** The [Developer](../seats/developer.md) seat has **no KPI named at all**, and a change that writes one for it is a miss.

**4. Check that named gaps stayed named.** If the change filled one in, **that is the miss** — say which gap, quoting [SOURCES.md](../../SOURCES.md) in the words that list already uses. The ones that get filled in most often: a holder for one of the twenty-three leftover-file seats, all of which **stay UNASSIGNED**; a speaking calendar, a Pendulum wiki, or a KPI behind one of them; a pipeline or a lead for the three unassigned Demand and Sales seats; and a second COO read out of the Persona Architect leftover.

**5. Read the last-gate lines the change will have to pass anyway.** [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md), so a fixable miss does not reach the PA as a surprise. You are reading those lines, not running the gate — that is the PA's step.

**6. Say pass, or name the miss.** One layer, one verdict, in plain words. **Do not add a second stamp** to something a C-suite seat already QC'd on its own function — crossed-seat sign-off is a miss, not a pass, and a stamp on top of a stamp is not QC. **Do not rewrite the page.** Fixing it is the producing seat's job; that seat is closer to the work than you are, and a QC that turns into a rewrite means nobody QC'd the result. There are no severity tiers here, no nits, and no partial verdict: it passes, or a named miss goes back.

A miss goes back to the seat that produced it and **does not travel on a promise to clean it up later**. Later is where a miss goes to be forgotten.

**7. Hand a pass on to the [PA](../seats/pa.md)**, and stop. The last gate and the merge happen after you, never instead of you.

**8. Stay silent to Michael on a routine pass.** A pass produces no ping either way. He hears about it when a QC failure blocks a sourced slice, or when the item is already on the ask-Michael-first list in [locks.md](../locks.md) — a number where the ladder shows both, a client's status, one of Cornelia Choe's two Zoom URLs, a Role for Jhana or Bob, or anything that would change that file. Those travel up the same wire to the PA, which is the seat that hands things to Michael. **You do not message Michael from this seat.**

**9. Stop, and write the note below.**

## The note you leave

Where the work is — on the pull request, or in the message back to the seat that produced the change. Four lines, and nothing more:

- **Where things stand.** One sentence somebody who was not here can act on.
- **The one change I QC'd**, the verdict, and where it went: on to the PA for the last gate, or back to the seat that produced it with a named miss.
- **What is still open**, each with its actual next step. "Follow up" is not a next step.
- **What I could not answer**, in this repo's own words: not recorded.

Two things make that note worth reading. **Never invent a name, an owner, a date, a figure, or a link to make a line look finished** — an unknown left as an unknown is the useful answer, and a plausible filler reads to the next person as something you checked. And **never quietly drop an item the last note left open**: if it closed, say it closed; if it did not, carry it forward.

No stamps, no status tags, no run identifiers. A person reads this.

## Stops that count as finished

A pass that stops honestly is a finished pass, not a failed one. Five of them:

- **A lock bit.** Quote it from [locks.md](../locks.md), in its own words. The change fails QC on that line.
- **A named gap got filled in.** Quote the hole from [SOURCES.md](../../SOURCES.md), in the words that list already uses, and hand it back.
- **The change came from a seat that does not own the work.** Name the owner's row and hand it back. Do not QC it anyway.
- **Nothing arrived to QC.** Say so. An empty in-tray is a real answer, and writing a page to check is not.
- **The item is an ask-Michael-first one.** It goes up the wire to the PA. You name it and stop there.

Either way you write the note. **A block is not permission to invent work**, and it is not permission to rewrite the page yourself.

## What this pass never does

- **Never merges, and never last-gates.** The PA does both, after you.
- **Never rewrites the work it is QC-ing.** Name the miss and hand it back.
- **Never signs off on a function this seat does not own**, and never stacks a stamp on another seat's QC.
- **Never pings Michael** to report a routine QC result, and never pings him instead of naming the lock or the hole.
- **Never sends.** No send without Michael — this seat is not an exception.
- **Never puts a figure in a KPI Current field.** Not a guess, not a target, not a 0. **Founder delivery hours %** and **Retreat fill rate** both stay empty.
- **Never invents a client, a price, a person, a Role, or a number**, and never names a second COO out of the Persona Architect leftover.
- **Never creates a meeting to fill a phase**, and never reads the existing calendar as an hours record.
- **Never touches program GitHub**, stands up a VM or a GKE cluster, installs a local model, or plans this pass around the M5. Full list: [locks.md](../locks.md).

## Named missing — stays named

- Detailed COO accountabilities beyond the public title. The title is sourced; the rest is not.
- Any COO SOP of its own.
- Any hours record, for Michael or for anyone else — so **Founder delivery hours %** has no denominator.
- Any next retreat: no date, guest list, or venue — so **Retreat fill rate** has nothing to fill.
- The KPI **Current** field on [plans/coo.md](../plans/coo.md) stays empty on both.

Full list, once, in [SOURCES.md](../../SOURCES.md). If a thing is named there, "not recorded" is the answer until Michael sources one.
