# Seat → job map

One table: for each of the 23 seats already written in [seats/](seats/README.md), which status it's in, which skill to open, and which Notion page backs that skill. This page adds no new seat, invents no new job, and rewrites nothing already in `seats/` — it's an index on top of facts already sourced there. Shape: the content-catalog table from [Workflowsio/company-os-starter-kit](https://github.com/Workflowsio/company-os-starter-kit) `blueprint/INDEX.md` — the same shape already used in [handbook/README.md](README.md) and [skills/README.md](../skills/README.md).

Each seat's own `run-<seat>` skill is listed first: it's the router that points at the seat page and hands off to the job skills beside it. Open the router, and it will tell you where the real work lives.

| Seat | Status | Open this skill | Open this Notion page |
|---|---|---|---|
| [PA](seats/pa.md) | Assigned | [run-pa](../skills/run-pa/SKILL.md) · [run-do-this](../skills/run-do-this/SKILL.md) · [author-support-reply](../skills/author-support-reply/SKILL.md) · [pa-handoff](../skills/pa-handoff/SKILL.md) | [Do this](https://app.notion.com/p/3c025e30d68b8142a971ccdb0d657b22) |
| [COO](seats/coo.md) | Assigned | [run-coo](../skills/run-coo/SKILL.md) · [run-always-on](../skills/run-always-on/SKILL.md) · [run-buyer-packet](../skills/run-buyer-packet/SKILL.md) | [Grok Bot staff](https://app.notion.com/p/3c125e30d68b81dc9116e2e62b47f143) |
| [CMO](seats/cmo.md) | Assigned | [run-cmo](../skills/run-cmo/SKILL.md) · [place-on-offer-ladder](../skills/place-on-offer-ladder/SKILL.md) · [run-sales-menu](../skills/run-sales-menu/SKILL.md) | [Sales Menu](https://app.notion.com/p/3c025e30d68b817dae2eeb55c5902ad7) |
| [Head of Content](seats/head-of-content.md) | Assigned | [competitive-writing-guide](../skills/competitive-writing-guide/SKILL.md) — router named missing, no `run-content` on main yet | [Competitive Writing Guide draft](https://app.notion.com/p/3c125e30d68b81239c5fc767bddc0823) |
| [Head of Demand](seats/head-of-demand.md) | Unassigned | [run-demand](../skills/run-demand/SKILL.md) | [Sales Menu](https://app.notion.com/p/3c025e30d68b817dae2eeb55c5902ad7) |
| [CSO](seats/cso.md) | Assigned | [run-cso](../skills/run-cso/SKILL.md) · [place-on-offer-ladder](../skills/place-on-offer-ladder/SKILL.md) · [run-sales-menu](../skills/run-sales-menu/SKILL.md) | [Sales Menu](https://app.notion.com/p/3c025e30d68b817dae2eeb55c5902ad7) |
| [Head of Sales](seats/head-of-sales.md) | Unassigned | [run-sales](../skills/run-sales/SKILL.md) · [run-uncovery](../skills/run-uncovery/SKILL.md) | [Uncovery SOP](https://app.notion.com/p/3c125e30d68b815d9dbbd7e59102af3e) |
| [SDR](seats/sdr.md) | Unassigned | [run-sdr-seat](../skills/run-sdr-seat/SKILL.md) · [campaign-lead-scoring](../skills/campaign-lead-scoring/SKILL.md) | [Campaign lead scoring draft](https://app.notion.com/p/3c125e30d68b81f89125cfbbe398c770) |
| [CFO](seats/cfo.md) | Assigned | [run-cfo](../skills/run-cfo/SKILL.md) · [run-money-moves](../skills/run-money-moves/SKILL.md) | [How money moves](https://app.notion.com/p/3c125e30d68b81b49524fe7bc9f65c81) |
| [Controller](seats/controller.md) | Assigned | [run-controller](../skills/run-controller/SKILL.md) · [run-money-moves](../skills/run-money-moves/SKILL.md) | [How money moves](https://app.notion.com/p/3c125e30d68b81b49524fe7bc9f65c81) |
| [Bookkeeper](seats/bookkeeper.md) | Assigned | [run-bookkeeper](../skills/run-bookkeeper/SKILL.md) · [run-money-moves](../skills/run-money-moves/SKILL.md) | [How money moves](https://app.notion.com/p/3c125e30d68b81b49524fe7bc9f65c81) |
| [CTO](seats/cto.md) | Assigned | [run-cto](../skills/run-cto/SKILL.md) | [Company OS home](https://app.notion.com/p/3c025e30d68b81cdbad7fdf5912e3ca3) |
| [Head of Engineering](seats/head-of-engineering.md) | Parked | [run-engineering](../skills/run-engineering/SKILL.md) | [Company OS home](https://app.notion.com/p/3c025e30d68b81cdbad7fdf5912e3ca3) |
| [Developer](seats/developer.md) | Parked | [run-developer](../skills/run-developer/SKILL.md) | [Company OS home](https://app.notion.com/p/3c025e30d68b81cdbad7fdf5912e3ca3) |
| [CCO](seats/cco.md) | Assigned | [run-cco](../skills/run-cco/SKILL.md) · [run-faq](../skills/run-faq/SKILL.md) · [last-gate-then-stop](../skills/last-gate-then-stop/SKILL.md) | [If a client writes](https://app.notion.com/p/3c025e30d68b81ada7b7cbf1d50b0d9f) |
| [Head of Author Success](seats/head-of-author-success.md) | Assigned | [run-author-success](../skills/run-author-success/SKILL.md) · [author-support-reply](../skills/author-support-reply/SKILL.md) · [support-call-prep](../skills/support-call-prep/SKILL.md) | [If a client writes](https://app.notion.com/p/3c025e30d68b81ada7b7cbf1d50b0d9f) |
| [Client Success](seats/client-success.md) | Assigned | [run-client-success](../skills/run-client-success/SKILL.md) · [run-faq](../skills/run-faq/SKILL.md) · [author-support-reply](../skills/author-support-reply/SKILL.md) | [If a client writes](https://app.notion.com/p/3c025e30d68b81ada7b7cbf1d50b0d9f) |
| [CHRO](seats/chro.md) | Assigned | [run-staff](../skills/run-staff/SKILL.md) — router named missing, no `run-chro` on main yet | [Grok Bot staff](https://app.notion.com/p/3c125e30d68b81dc9116e2e62b47f143) |
| [People Ops](seats/people-ops.md) | Assigned | [run-staff](../skills/run-staff/SKILL.md) — router named missing, no `run-people-ops` on main yet | [Grok Bot staff](https://app.notion.com/p/3c125e30d68b81dc9116e2e62b47f143) |
| [VP Campaigns](seats/vp-campaigns.md) | Assigned | [run-vp-campaigns](../skills/run-vp-campaigns/SKILL.md) · [run-campaign](../skills/run-campaign/SKILL.md) | [Campaign SOP](https://app.notion.com/p/3c025e30d68b81ea99c0dcf96db7cd2e) |
| [Campaign Coordinator](seats/campaign-coordinator.md) | Assigned | [run-campaign-coordinator](../skills/run-campaign-coordinator/SKILL.md) · [run-campaign](../skills/run-campaign/SKILL.md) · [run-sales-menu](../skills/run-sales-menu/SKILL.md) | [Campaign Coordinator do-this](https://app.notion.com/p/3c125e30d68b8181aaece1c83104102d) |
| [VP Retreats](seats/vp-retreats.md) | Assigned | [run-vp-retreats](../skills/run-vp-retreats/SKILL.md) · [run-retreat](../skills/run-retreat/SKILL.md) · [run-piab](../skills/run-piab/SKILL.md) · [blank-guest-intake](../skills/blank-guest-intake/SKILL.md) | [Retreat SOP](https://app.notion.com/p/3c025e30d68b8185b9a9f19dd56389e5) |
| [Retreat Producer](seats/retreat-producer.md) | Assigned | [run-retreat-producer](../skills/run-retreat-producer/SKILL.md) · [run-retreat](../skills/run-retreat/SKILL.md) · [blank-guest-intake](../skills/blank-guest-intake/SKILL.md) · [quote-track-record](../skills/quote-track-record/SKILL.md) | [Retreat SOP](https://app.notion.com/p/3c025e30d68b8185b9a9f19dd56389e5) |

## Two seats that are not one seat

- **Campaign Coordinator is not VP Campaigns.** [VP Campaigns](seats/vp-campaigns.md) owns the Campaign SOP; [Campaign Coordinator](seats/campaign-coordinator.md) runs the do-this page under it. Two rows, two routers.
- **Retreat Producer is not VP Retreats.** [VP Retreats](seats/vp-retreats.md) owns the Retreat and PIAB SOPs; [Retreat Producer](seats/retreat-producer.md) produces each retreat. Two rows, two routers.
- **CMO does not own campaign day-to-day**, and CSO is Chief Sales Officer — not Chief Strategy Officer. See [run-cmo](../skills/run-cmo/SKILL.md) and [run-cso](../skills/run-cso/SKILL.md).

## Every row, before you run it

- [last-gate-then-stop](../skills/last-gate-then-stop/SKILL.md) runs last on every job in this table, regardless of row — it isn't repeated in every cell because it applies to all of them.
- If a **price or a Sales Menu number** comes up on any row, run [place-on-offer-ladder](../skills/place-on-offer-ladder/SKILL.md) and [run-sales-menu](../skills/run-sales-menu/SKILL.md) rather than recalling a number.
- If the **track-record number** comes up on any row, run [quote-track-record](../skills/quote-track-record/SKILL.md) — quoted uncollapsed, each figure with its date or context.
- If a **client writes** on any row, [run-faq](../skills/run-faq/SKILL.md) says what the FAQ covers and [author-support-reply](../skills/author-support-reply/SKILL.md) drafts it. Nobody sends.
- If a **person** question comes up on any row, [run-staff](../skills/run-staff/SKILL.md) answers it from the recorded roster.
- [reuse-what-github-has](../skills/reuse-what-github-has/SKILL.md) runs before anyone writes the missing router for a row above — search public GitHub first, adapt the shape, name what you reused in [SOURCES.md](../SOURCES.md). Do not invent a router to close a gap in this table.
- [handbook/cheap-loop.md](cheap-loop.md) is the loop this whole table plugs into: open the skill in the row, follow it, gate, stop.

## Locked, regardless of row

- **No send without Michael**, on any row, however clean the draft looks.
- **No program GitHub** from any row — `smarter-voice`, `academic-research-platform`, `book-campaign-platform`, `styleguide-os`, `persona-standalone-programs`, `tlpF-b01-research-engine`.
- **Demand, Sales, and SDR stay unassigned.** [run-demand](../skills/run-demand/SKILL.md), [run-sales](../skills/run-sales/SKILL.md), and [run-sdr-seat](../skills/run-sdr-seat/SKILL.md) exist to answer honestly about those seats — no inbound volume, pipeline, forecast, lead count, or score is invented for them.
- **CTO, Head of Engineering, and Developer stay under the machine locks.** No VMs, no GKE, no local LLM; M5 stays parked until the machine is physically in hand. Dave / Lehi Drew is a **vendor**, not a seat holder.
- **Jhana and Bob have no Role recorded.** No row on this page assigns them one.
- **Cornelia Choe is Alumni — support, not a pitch.** Her two Zoom URLs stay unresolved; flag both rather than picking one.
- **KPI Current stays empty** — 0 Current, 0 Prospect per the 18 Aug 2026 extract in [clients.md](clients.md).
- **Prices:** quote both numbers where the ladder shows two, and Platinum Major List has no public price. See [offers.md](offers.md).

Full list: [locks.md](locks.md).

## Named missing

Three seats have no dedicated router yet: **Head of Content** (no `run-content`), **CHRO**, and **People Ops** (no `run-chro`, no `run-people-ops`). Each row above points at the closest skill that genuinely exists — `competitive-writing-guide` for the writing-guide draft Head of Content owns, `run-staff` for the roster CHRO and People Ops own — and names the missing router instead of inventing one. Full list of every named gap in this repo: [SOURCES.md](../SOURCES.md).
