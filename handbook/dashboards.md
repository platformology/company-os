# Dashboards — what we can actually show, and what we can't

This is not a dashboard. It is the page that says why there isn't one yet, what is genuinely blocking each number, and what a useful dashboard would show on the day those blocks lift. Nobody builds a chart off this page, and nobody fills a figure in to make it look finished.

Read [locks.md](locks.md) first, like everything else here.

## The three that get asked for most, and where each one actually stands

**KPI "Current" is empty, and it stays empty.** No figure goes in that field — and a 0 is a figure, so a 0 does not go in either. The live KPI page is in Notion and [run-kpis](../skills/run-kpis/SKILL.md) is the skill that opens it; this repo does not restate what is on it. The 18 Aug 2026 extract in [clients.md](clients.md) separately counts 1 Alumni, 67 Past, 0 Current, and 0 Prospect. **That count is a different fact from the KPI field**, quoted with its extract date, and it does not get carried across to fill the blank. It changes when Michael sources a figure.

**HubSpot is closed.** It is not a system of record, it is not a live CRM, and nothing gets read out of it into a chart. The CRM is Notion Clients — see [clients.md](clients.md). A folder name is not a client, and a Past client is not a Current one.

**Bench has no connector.** There is no wire from Bench to this Mac, so no ledger figure, no savings total, and no cash number comes off it here. That is recorded on [runtime-body.md](runtime-body.md) as a denied hand for the money seats, and in [SOURCES.md](../SOURCES.md) as a named gap. June and July 2026 are also not closed — see [seats/controller.md](seats/controller.md) — so even a hand-built monthly view would be reporting on months the Controller has not signed off.

## What a useful dashboard would show, once each line is sourced

Nothing below exists today. This is the ask list, not a spec to go implement, and no row gets estimated, benchmarked, or filled from a similar company.

| What it would show | What has to be true first |
|---|---|
| Current clients, live | Michael sources a Current figure for the KPI field, and Hoffman's status stops being a question — see [clients.md](clients.md) |
| Pipeline and close | [Head of Sales](seats/head-of-sales.md) and [SDR](seats/sdr.md) stop being unassigned, and there is a real pipeline to read. No forecast is invented for empty seats |
| Cash and monthly close | A Bench connector exists, and June and July 2026 are closed by the [Controller](seats/controller.md) |
| Campaign and retreat delivery | A live campaign or retreat exists to report on. A retreat date, guest list, and venue are all named missing |
| Content and corpus coverage | The [Head of Content](seats/head-of-content.md) catalog is far enough along to count against — cataloged, not written |
| Seats filled | People get recorded in [people.md](people.md). Today that reads three people and two vendors, and 45 of 46 seats have no holder recorded |

Each row is one honest sentence when someone asks for it today: **not sourced, here is what would have to exist.** That answer is the deliverable until it isn't.

## What nobody builds off this page

- **No home-built dashboard.** [runtime-wiring.md](runtime-wiring.md) already settles this: a dashboard is a thing to maintain, the seats' own Grok Bot chats are the wire, and nobody installs a board, a bus, or a dashboard to make the wiring work. This page does not reopen that.
- **No screenshot of a chart with placeholder numbers in it**, and no "example" dashboard. A placeholder figure gets screenshotted into a deck within a week, and then nobody can tell it from a real one.
- **Nothing installed to render it.** No VMs, no GKE — see [locks.md](locks.md). This repo is markdown.
- **No external report.** Anything that would go to a client, a prospect, or a buyer passes [reviews/last-gate-checklist.md](../reviews/last-gate-checklist.md) and stops with Michael. No send without Michael.

## Named missing

- KPI "Current" — stays empty until Michael sources a figure.
- Bench connector, and any savings or ledger total off it.
- June and July 2026 closes.
- Any pipeline, forecast, inbound volume, lead count, or conversion rate — Demand, Sales, and SDR are unassigned, and the 23 seats named on 20 Aug 2026 are unassigned too.
- Which social accounts exist, and any audience or engagement figure — see [seats/social-media-strategist.md](seats/social-media-strategist.md).
- Any site, analytics account, keyword, or ranking figure — see [seats/seo-expert.md](seats/seo-expert.md).
- Any speaking calendar, event, or fee — see [seats/speaking-universities.md](seats/speaking-universities.md) and [seats/speaking-associations.md](seats/speaking-associations.md).

The full list of every named gap in this repo is in [SOURCES.md](../SOURCES.md). Nothing on it gets filled in from memory or from a reasonable guess.
