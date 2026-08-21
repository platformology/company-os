# Bookkeeper — plan

**Status: Assigned** · **Holder: not recorded** · **Written: 20 Aug 2026**

One pass on a bill or a ledger question, with Bench read as the ledger and never as a live feed.

## Open these first, in this order

1. [locks.md](../locks.md).
2. [seats/bookkeeper.md](../seats/bookkeeper.md) — the seat page. If this plan and that page ever disagree, the seat page wins.
3. [desks/bookkeeper.md](../desks/bookkeeper.md) — the sit-down pack.
4. [run-bookkeeper](../../skills/run-bookkeeper/SKILL.md) — the router for this seat.
5. [how-money-moves.md](../how-money-moves.md) — where bills sit among the five money jobs.

## The one job

**Answer or advance one bills-or-ledger question, and where the number is not in hand, say it is not in hand.**

Bench is the Platformology general ledger. **No Bench connector exists in this repo or its skills** — there is nothing here that pulls from it, so a figure that would have to come from a live pull is a figure you do not have. This seat's live leftover is exactly that: **any savings total is not sourced, and it does not get invented.**

## The SOP that runs it

[How money moves](https://app.notion.com/p/3c125e30d68b81b49524fe7bc9f65c81) (Notion) is the page this seat's row in [seat-job-map.md](../seat-job-map.md) names, and [Company OS home](https://app.notion.com/p/3c025e30d68b81cdbad7fdf5912e3ca3) (Notion) is what the seat page names. **There is no bookkeeping SOP of its own recorded in this repo — named missing**, and no generic accounts-payable checklist gets written in to cover the hole.

## The KPI this plan is pointed at

| | |
|---|---|
| **KPI** | **Bills and collections.** Already named on the C-suite operating plan; copied here as a name, nothing more. |
| **Current** | **Empty.** No figure has been sourced for that field, and none goes in it — not an amount outstanding, not a count of open bills, not a 0. **A 0 is a figure.** |
| **Do not confuse it with** | The client count. The 18 Aug 2026 extract in [clients.md](../clients.md) counts 0 Current and 0 Prospect. That is a client count with a date on it, not a collections figure, and the two do not get joined. |
| **Where it lives** | [KPIs](https://app.notion.com/p/b104782240524af595577abaef8dc928) (Notion). This repo does not restate the dashboard — see [run-kpis](../../skills/run-kpis/SKILL.md). |

## Run it

1. Open [locks.md](../locks.md). No invented revenue, savings, or Current numbers, on any pass.
2. Take the question. If it is a **bill** — is it paid, is it due, who is it from — answer from the record, and where the record is not in hand, say the record is not in hand.
3. If it is a **collections** question, the same rule holds. No accounts-receivable figure is recorded in this repo, so none gets quoted from here.
4. If it is a **Bench** question: Bench is the general ledger. There is **no connector**, so this seat does not report a live balance, a savings total, or a trend off it. Say what Bench is and what is not wired to it.
5. An invoice, payment, or payout that actually needs running goes through [run-money-moves](../../skills/run-money-moves/SKILL.md).
6. A monthly-close question is not this seat's — hand it to [Controller](../seats/controller.md). **June and July 2026 are not closed.**
7. Hand the finished thing to the [CFO](../seats/cfo.md), who owns the function bills and the ledger sit inside — see [runtime-wiring.md](../runtime-wiring.md).
8. Run [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md) and stop.

## Done looks like

One bill or ledger question is answered from a record, or is plainly named as unanswerable from what is recorded here. No savings total, no Bench balance, and no receivable figure appeared. The KPI field is still empty.

## Named missing — stays named

- Who currently fills this seat.
- Any savings total — not sourced, not invented.
- No Bench connector.
- Any bookkeeping SOP of its own.
- No invented invoice or accounts-receivable figure.

## Never

- Never report a live Bench pull. There is no connector, and describing one as if there were is inventing a system.
- Never state a savings total, a balance, or an outstanding-receivables figure that is not in a record you actually opened.
- Never write a figure into KPI Current, including a 0.
- Never invent revenue, and never attach a revenue figure to an offer — none on [offers.md](../offers.md) has one.
- Never send without Michael. No program GitHub. See [locks.md](../locks.md).
