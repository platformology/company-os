# Runtime body — the hands each assigned seat already has

One table: for every **assigned** seat, the skill it opens, the tools on this Mac it is allowed to touch, and what "body done" looks like for it. The seat's job is already written in [seats/](seats/README.md) and its route is already in [seat-job-map.md](seat-job-map.md); this page restates neither. It answers a different question — **does the seat have hands, and which ones.**

Michael, 19 Aug 2026: each assigned bot needs skills **and** tools on this Mac. Pages are not the person.

The map this page sits under is `handbook/runtime.md` — in flight, not landed in this repo yet.

Shape: a role-permissions table searched on public GitHub first — each row says what the role may touch, granted or **explicitly denied**, and the seat is tracked separately from whoever fills it. Kit URLs stay off this page; the reused shape is named in the pull request that landed it, and its [SOURCES.md](../SOURCES.md) row is a leftover below.

## What "has a body" means

Three things, all three, or the seat has a page and no body:

1. **The skill is on this computer** — the seat's router in [skills/](../skills/README.md), openable, not described.
2. **The tools in its row are the only hands it has.** Not preferred tools — the whole set. A tool that is not in the row is not that seat's to touch.
3. **The seat can run its own router** — without the [PA](seats/pa.md) writing the page for it first.

A body is not a permission to send. **No send without Michael** — see [locks.md](locks.md).

## The five tools connected to this Mac

Notion (Company OS, Clients, Team, KPIs, SOPs) · Gmail · Google Calendar (michael@profluent.com, America/Denver) · Slack · Google Drive.

That is the whole set, and nothing gets installed to make a row below work:

- **No HubSpot.** It is closed and is not a system of record — see [clients.md](clients.md).
- **No Apple Contacts connector.**
- **No Bench connector.** Bench is the general ledger and nothing on this Mac reads it — see [seats/bookkeeper.md](seats/bookkeeper.md).
- **No new CRM.** The CRM is Notion Clients.
- **Slack is connected and no seat's job in this repo sources it**, so no row below claims it. That is a leftover for Michael to assign, not a gap to fill by inventing a channel.

Two "Drive"s, one word: **Google Drive** is a tool on this Mac. **"Drive"** on the offer ladder is how a price gets paid — see [offers.md](offers.md). Don't read one as the other.

## Assigned seats

The Notion URLs are already in [seat-job-map.md](seat-job-map.md) and on the seat pages, so this page names each Notion page rather than re-linking it. One router skill per row — the rest of a seat's skills are on that same map.

| Seat | Open this skill | Hands on this Mac | Body done when |
|---|---|---|---|
| [PA](seats/pa.md) | [run-pa](../skills/run-pa/SKILL.md) | Notion **Do this**. Google Calendar — read the existing :08/:38, :13/:43, :23/:53 slots and the daily PA + COO triage. Gmail — read, and draft in Michael's own accounts. *Denied:* sending anything. | It works today's list off **Do this**, reads the cadence off the calendar instead of asking for it, and hands every draft to Michael. |
| [COO](seats/coo.md) | [run-coo](../skills/run-coo/SKILL.md) | Notion **Grok Bot staff**, **Do this**, **Company OS home**, **Buyer data room**. Google Calendar — read the meetings that already exist. *Denied:* creating a meeting to fill a phase. | It runs one pass (plan, meetings, execution, QC) off those pages and the existing calendar, and the QC pass stays silent to Michael. |
| [CMO](seats/cmo.md) | [run-cmo](../skills/run-cmo/SKILL.md) | Notion **Sales Menu**; [offers.md](offers.md) in this repo. *Denied:* any demand tool — Head of Demand is leftover-file assigned; who fills it is not recorded; there is no live job. | It quotes the ladder off the Sales Menu, both numbers where two are written, and does not invent a live job for leftover-file assigned Demand. |
| [Head of Content](seats/head-of-content.md) | [run-content](../skills/run-content/SKILL.md) | Google Drive and the existing files — find what the corpus already holds. Notion **Buyer data room**, **Competitive Writing Guide draft**. *Denied:* writing new copy and filing it as corpus. | It can say where a corpus piece is, or that it isn't in hand, without composing a stand-in. |
| [CSO](seats/cso.md) | [run-cso](../skills/run-cso/SKILL.md) | Notion **Sales Menu**, Notion **Clients** for status; [offers.md](offers.md), [clients.md](clients.md). *Denied:* any pipeline tool — Head of Sales and SDR are leftover-file assigned; who fills each is not recorded; there is no live job. | It places someone on an existing rung from the menu and answers "no pipeline recorded" rather than producing a forecast. |
| [CFO](seats/cfo.md) | [run-cfo](../skills/run-cfo/SKILL.md) | Notion **How money moves**. *Denied:* Bench — no connector exists. | It runs a money question off **How money moves**, and any ledger figure is either attributed to someone opening Bench or named missing. |
| [Controller](seats/controller.md) | [run-controller](../skills/run-controller/SKILL.md) | Notion **How money moves**. *Denied:* Bench — no connector exists. | It says June and July 2026 are not closed, with no close invented and nothing written into KPI Current. |
| [Bookkeeper](seats/bookkeeper.md) | [run-bookkeeper](../skills/run-bookkeeper/SKILL.md) | Notion **How money moves**. *Denied:* Bench — no connector, so Bench is opened by hand or not at all. | It says what it actually did — opened Bench and read it, or didn't — and reports no savings total. |
| [CTO](seats/cto.md) | [run-cto](../skills/run-cto/SKILL.md) | Notion **Company OS home**; [locks.md](locks.md). *Denied:* installing anything — no local LLM, no VM, no GKE. Work runs on this Mac. Machine locks live on [locks.md](locks.md). | The desk is the five tools above and nothing else, and the seat names the lock that blocks an ask and stops there. |
| [CCO](seats/cco.md) | [run-cco](../skills/run-cco/SKILL.md) | Notion **If a client writes** (the FAQ); [clients.md](clients.md). Gmail — read what came in. *Denied:* sending. | It reads the inbound in Gmail, answers only what the FAQ covers, and every draft stops with Michael. |
| [Head of Author Success](seats/head-of-author-success.md) | [run-author-success](../skills/run-author-success/SKILL.md) | Notion **If a client writes**. Gmail — read. Google Calendar — read an existing call's time. *Denied:* sending. | It preps off the FAQ and the calendar, and says "Not in the FAQ — flag for Michael before sending" instead of filling the hole. |
| [Client Success](seats/client-success.md) | [run-client-success](../skills/run-client-success/SKILL.md) | Notion **If a client writes**. Gmail — read and draft. *Denied:* sending, posting, scheduling, or replying directly. | The day-to-day draft exists in Gmail and leaves only when Michael sends it. |
| [CHRO](seats/chro.md) | [run-chro](../skills/run-chro/SKILL.md) | Notion **Team** / **Grok Bot staff**; [people.md](people.md). *Denied:* recording a Role for Jhana or Bob. | It answers a person question off the recorded roster — Jhana, Bob, Anthony C. Garcia — and vendors stay vendors. |
| [People Ops](seats/people-ops.md) | [run-people-ops](../skills/run-people-ops/SKILL.md) | Notion **Team** / **Grok Bot staff**; [people.md](people.md). *Denied:* editing the roster — a change is drafted for Michael. | The roster stays honest: no Role for Jhana or Bob, no rate or term added to a vendor, no seat holder filled in from a guess. |
| [VP Campaigns](seats/vp-campaigns.md) | [run-vp-campaigns](../skills/run-vp-campaigns/SKILL.md) | Notion **Campaign SOP** — the SOP this seat owns. | It answers an ownership question off the SOP and hands day-to-day down to the Coordinator. |
| [Campaign Coordinator](seats/campaign-coordinator.md) | [run-campaign-coordinator](../skills/run-campaign-coordinator/SKILL.md) | Notion **Campaign Coordinator do-this**, and the **Campaign SOP** to read. | Work that isn't on the do-this page isn't this seat's job, and the seat can say that out loud. |
| [VP Retreats](seats/vp-retreats.md) | [run-vp-retreats](../skills/run-vp-retreats/SKILL.md) | Notion **Retreat SOP**, **PIAB SOP**, **blank guest intake draft**. | It decides off those two SOPs, and date, guest list, venue, and the blank intake fields stay named missing. |
| [Retreat Producer](seats/retreat-producer.md) | [run-retreat-producer](../skills/run-retreat-producer/SKILL.md) | Notion **Retreat SOP**, **blank guest intake draft**. | It produces one retreat off the SOP, quotes the track-record numbers uncollapsed, and invents no date, guest, or venue. |

Three notes the rows are too narrow to hold:

- **Money seats.** [CFO](seats/cfo.md), [Controller](seats/controller.md), and [Bookkeeper](seats/bookkeeper.md) share one page — Notion **How money moves** — and one missing hand. Bench is named missing as a connector, so no spend, savings, or balance figure comes off this Mac.
- **Customer seats.** [CCO](seats/cco.md), [Head of Author Success](seats/head-of-author-success.md), and [Client Success](seats/client-success.md) read in Gmail and answer from the **If a client writes** FAQ. Cornelia Choe is our 1 Alumni — support, not a pitch — and the 18 Aug 2026 extract counts 0 Current and 0 Prospect ([clients.md](clients.md)). Nobody sends without Michael.
- **CTO.** Michael's 19 Aug 2026 note names three things for this seat: locks, desk, go packet. The locks are in [locks.md](locks.md); the desk is the five connected tools; the **go packet is not written down in this repo**, so it stays a leftover rather than something this page drafts.

## Parked — no body, no live work

- **[Head of Engineering](seats/head-of-engineering.md)** — parked. [run-engineering](../skills/run-engineering/SKILL.md) exists to answer about the seat and refuse work from it; no tool on this Mac is assigned to it, and the machine locks are why.
- **[Developer](seats/developer.md)** — parked under the same locks. [run-developer](../skills/run-developer/SKILL.md) answers about the seat; there is no recorded stack or machine to write code on, so there is nothing to hand it.

## Leftover-file assigned — leftover already written, no live job

- **[Head of Demand](seats/head-of-demand.md)** — leftover-file assigned. Who fills it is not recorded. There is no live job. The leftover it opens is already written: [leftovers/head-of-demand.md](leftovers/head-of-demand.md). [run-demand](../skills/run-demand/SKILL.md) exists to answer honestly about the seat; no inbound volume, channel, or lead is invented, and [CMO](seats/cmo.md) does not invent a live job for this seat.
- **[Head of Sales](seats/head-of-sales.md)** — leftover-file assigned. Who fills it is not recorded. There is no live job. The leftover it opens is already written: [leftovers/head-of-sales.md](leftovers/head-of-sales.md). [run-sales](../skills/run-sales/SKILL.md) exists to answer honestly about the seat; no pipeline, forecast, or close rate exists to report, and [CSO](seats/cso.md) does not invent a live job for this seat.
- **[SDR](seats/sdr.md)** — leftover-file assigned. Who fills it is not recorded. There is no live job. The leftover it opens is already written: [leftovers/sdr.md](leftovers/sdr.md). [run-sdr-seat](../skills/run-sdr-seat/SKILL.md) exists to answer honestly about the seat; no lead list, lead count, or score exists behind it.

## Done-check for one seat's body

Run it out loud, on the seat in front of you:

1. **Is the router skill on this computer?** A folder in [skills/](../skills/README.md) is the check — every assigned row above has one.
2. **Are the tools in its row the only ones it touched?** A tool outside the row is a stop, not an improvisation.
3. **Did the seat run its own router**, without the PA writing the page for it?

What this repo cannot check: whether a skill is **installed on the Mac as a Grok workflow.** The folder existing here is not that, and this page does not claim it — see the leftovers below.

## Locked on every row above

**No send without Michael.** No program GitHub. Nothing installed — no VM, no GKE, no local LLM. Work runs on this Mac. Machine locks live on [locks.md](locks.md) — this page does not restate them. Prices only from [offers.md](offers.md), both numbers where the ladder shows two. KPI Current stays empty, and the 0 Current / 0 Prospect client counts go out with their 18 Aug 2026 extract date. Cornelia Choe is Alumni — support, not a pitch. Full list: [locks.md](locks.md), and the cheap loop every row runs inside: [cheap-loop.md](cheap-loop.md).

## Leftovers

- Index this file from the map when `handbook/runtime.md` lands.
- Confirm each router skill above is installed on the Mac as a Grok workflow — PA, from the Mac, since this repo can't show it.
- Slack is connected and assigned to no seat's job; Michael names the job that uses it, or it stays unused.
- This page's reused shape has no row in [SOURCES.md](../SOURCES.md) yet; whoever next edits that file should add one.
