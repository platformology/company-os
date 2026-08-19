---
name: run-kpis
description: Point to the KPIs Notion page and the 18 Aug 2026 client extract — never invent a Current number, a savings total, or offer-level revenue. Use when asked to check, report, or update a Platformology KPI.
---

# Run KPIs

Reused from: [narrative-io/narrative-skills-marketplace](https://github.com/narrative-io/narrative-skills-marketplace), `docs/authoring-skills.md` ("never duplicate" the reference in the skill body), and [dzhng/skills](https://github.com/dzhng/skills), `skills/authoring/write-skills/SKILL.md` ("keep a single source of truth") — the same point-and-stop pattern already used by [run-money-moves](../run-money-moves/SKILL.md) and [pa-handoff](../pa-handoff/SKILL.md).

## The gate

Two sources back a KPI check; this skill does not restate either:

- [KPIs](https://app.notion.com/p/b104782240524af595577abaef8dc928) (Notion) — the live dashboard.
- [handbook/clients.md](../../handbook/clients.md) — the 18 Aug 2026 extract: 1 Alumni (Cornelia Choe), 67 Past, 0 Current, 0 Prospect.

## KPI Current stays empty

**Do not invent a Current number.** 0 Current is the sourced fact from the 18 Aug 2026 extract — not a placeholder waiting for a bigger one. See [handbook/clients.md](../../handbook/clients.md).

## Steps

1. Open [KPIs](https://app.notion.com/p/b104782240524af595577abaef8dc928) before reporting anything — this repo does not restate the dashboard.
2. Cross-check any client count against [handbook/clients.md](../../handbook/clients.md): 1 Alumni, 67 Past, 0 Current, 0 Prospect (18 Aug 2026 extract).
3. **Do not invent a Current number, a savings total, or an offer-level revenue figure.** None of those is sourced in this repo — see [handbook/how-money-moves.md](../../handbook/how-money-moves.md) and [SOURCES.md](../../SOURCES.md).
4. **Hoffman is a question, not a fact.** Do not count Hoffman toward Current, Past, or Prospect — see [handbook/clients.md](../../handbook/clients.md).
5. **The CRM is Notion Clients. HubSpot is closed** — don't pull a KPI from it, and don't treat a folder name as a client. See [handbook/clients.md](../../handbook/clients.md).
6. Hand the question to the seat that owns it rather than answering past your row: a **monthly close** question is [run-controller](../run-controller/SKILL.md) (June and July 2026 are not closed), **Bench or a savings figure** is [run-bookkeeper](../run-bookkeeper/SKILL.md), and the **track-record number** is [quote-track-record](../quote-track-record/SKILL.md) — not a KPI to collapse into one figure.
7. Before anything drawn from a KPI check goes anywhere external, run it through [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md).

## Never

- Never invent a Current number — it stays empty/0 per the sourced 18 Aug 2026 extract.
- Never treat HubSpot as a live system of record — it's closed; the CRM is Notion Clients.
- Never invent a savings total or a Bench connector — see [handbook/seats/bookkeeper.md](../../handbook/seats/bookkeeper.md).
- Never invent offer-level revenue — no offer in [handbook/offers.md](../../handbook/offers.md) has a revenue figure attached to it.
- Never record Hoffman as Current.
- Never send a KPI report without Michael. See [handbook/locks.md](../../handbook/locks.md).
