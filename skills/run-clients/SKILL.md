---
name: run-clients
description: Point to handbook/clients.md and the Notion Clients database — never invent a live client, an offer, a revenue figure, or an outcome. Use when someone asks who the clients are, wants to add a client or change a client's status, or treats a folder name as a client.
---

# Run clients

Reused from: [narrative-io/narrative-skills-marketplace](https://github.com/narrative-io/narrative-skills-marketplace), `docs/authoring-skills.md` ("never duplicate" the reference in the skill body), [dzhng/skills](https://github.com/dzhng/skills), `skills/authoring/write-skills/SKILL.md` ("keep a single source of truth"), and [slgoodrich/agents](https://github.com/slgoodrich/agents), `plugins/ai-pm-copilot/skills/competitive-analysis-templates/SKILL.md` ("never fabricate... when data is unavailable, explicitly note it rather than inventing data"). All three are already credited in [`SOURCES.md`](../../SOURCES.md). This is the same point-and-stop shape as [run-kpis](../run-kpis/SKILL.md) and [run-money-moves](../run-money-moves/SKILL.md).

## The gate

Two things answer a client question, and this skill restates neither:

- [handbook/clients.md](../../handbook/clients.md) — the 18 Aug 2026 extract: 1 Alumni (Cornelia Choe, The Leaders Alliance), 67 Past, 0 Current, 0 Prospect.
- **Notion Clients** — the CRM, and the only place a client record is created or changed. This repo carries counts, not records.

**HubSpot is closed.** It is not the CRM and not a system of record. Do not open it to settle a client question, and do not migrate anything out of it on your own.

This repo does not record a link to the Notion Clients database. Find it in Notion or ask Michael — do not substitute a folder, a HubSpot export, or a search result for it.

## The three asks this skill covers

| Someone asks | The honest move |
|---|---|
| "Who are our clients?" | Read the counts off [handbook/clients.md](../../handbook/clients.md), name the extract date, and stop. The Current client count is 0 on the 18 Aug 2026 extract, and that is the answer, not a gap to fill. The KPI "Current" is a different field, and it stays empty. |
| "Add a client" / "move this one to Current" | The record is created in Notion Clients, and a status change is an ask-Michael-first item — see [handbook/locks.md](../../handbook/locks.md). Don't edit `clients.md` to make it true. |
| "This folder is named X, so X is a client" | No. **Folder names are not clients** — not past, not current, not prospect. A folder is a folder. |

## Steps

1. Open [handbook/clients.md](../../handbook/clients.md) before answering anything. Every count you give carries its extract date: 18 Aug 2026.
2. If the ask is about a specific record — history, notes, contact details — that lives in Notion Clients, not here. Go there rather than reconstructing it.
3. **The Current client count is 0 and stays 0** until Michael sources a change. Asked how many current clients there are, 0 with the 18 Aug 2026 extract date is the honest answer. The KPI "Current" is a different field, and it stays empty — do not fill it with the client count, or with anything else. See [run-kpis](../run-kpis/SKILL.md).
4. **Hoffman is a question, not a Current client.** Leave it a question. Do not count Hoffman toward Current, Past, or Prospect.
5. **There are no 2021–2026 current clients to be found without Michael's files.** If asked to reconstruct recent client history, say the files aren't here rather than assembling a list from folders, past clients, or memory.
6. Adding or reactivating a client, or moving anyone to Current or Prospect, stops at Michael — [handbook/locks.md](../../handbook/locks.md).
7. Before anything built on a client fact leaves the building, run [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md), then stop.

## Cornelia Choe

Our one Alumni relationship, The Leaders Alliance. Her project is done and we are still supporting her.

- Her **Thu 20 Aug 2026, 11:00–11:30am America/Denver** meeting is **support, not a pitch.** Nothing prepared for it carries an offer, a price, or an upsell.
- **Two Zoom URLs exist for that meeting and neither is resolved.** Flag both to Michael. Do not pick one, and do not send either.
- Prepping the call is [support-call-prep](../support-call-prep/SKILL.md). A written reply to her is [author-support-reply](../author-support-reply/SKILL.md) — draft only.

## Named missing

- A link to the Notion Clients database is not recorded in this repo.
- Hoffman's status — a question, not a fact.
- The two unresolved Zoom URLs for Cornelia's 20 Aug 2026 meeting.
- Michael's files for 2021–2026, without which there is no current-client history to give.

## Never

- Never invent a live client, an offer, a revenue figure, or an outcome for any account.
- Never treat a folder name as evidence of a client.
- Never record Hoffman as Current.
- Never treat HubSpot as the CRM — it is closed.
- Never invent a Current number to make the roster look busier. What's sourced is the client count — 0 Current on the 18 Aug 2026 extract — and it goes out with that date.
- Never restate the Notion Clients database or `clients.md` inside another page — link them, and keep one source of truth.
- Never send anything to a client, and never pick between Cornelia's two Zoom URLs. No send without Michael. No program GitHub. See [handbook/locks.md](../../handbook/locks.md).
