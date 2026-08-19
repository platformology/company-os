---
name: run-bookkeeper
description: Run the Bookkeeper seat by pointing at handbook/seats/bookkeeper.md — never restate it, and never report a savings total. Use when a bill needs paying or checking, or when someone asks about Bench, the general ledger, or what a bill saved.
---

# Run the Bookkeeper seat

Reused from: [narrative-io/narrative-skills-marketplace](https://github.com/narrative-io/narrative-skills-marketplace), `docs/authoring-skills.md` ("never duplicate" the reference in the skill body), and [dzhng/skills](https://github.com/dzhng/skills), `skills/authoring/write-skills/SKILL.md` ("keep a single source of truth").

## The gate
[handbook/seats/bookkeeper.md](../../handbook/seats/bookkeeper.md) is the seat. This skill points at it and does not restate it. The seat keeps the bills paid and the general ledger accurate, and it reports to [CFO](../../handbook/seats/cfo.md) — see the [run-cfo](../run-cfo/SKILL.md) skill.

**The seat holder is not recorded** — see [handbook/people.md](../../handbook/people.md).

## Bench, and what it isn't
**Bench is the Platformology general ledger.** **No Bench connector exists** in this repo or in any skill in it.

So nothing here reads Bench, and nothing here can. Any ledger figure — a balance, a category total, a vendor total, a savings total — comes from opening Bench itself, and it gets attributed to that read. It never comes from this repo, and it is never reconstructed from memory.

## Steps
1. Open [handbook/seats/bookkeeper.md](../../handbook/seats/bookkeeper.md) before touching a bill or quoting a ledger figure.
2. **Bills:** work the actual bill in front of you. This repo records no vendor list, no bill amounts, no payment schedule, and no approval thresholds — if the bill doesn't say it, it is a question for Michael, not an assumption.
3. **Do not report a savings total.** There isn't one in this repo, it is a named missing in [SOURCES.md](../../SOURCES.md), and "roughly" or "about" is still an invented number. If asked what was saved, the answer is that no savings total is sourced.
4. **Do not invent a live pull from Bench.** There is no connector; say what you actually did — opened Bench and read it, or didn't.
5. **Do not invent an invoice or an accounts-receivable figure.** Neither is sourced here.
6. **Blue Sky stays off the LLC books.** Platformology LLC is the legal entity; Promote a Book and Book Retreat are DBAs of it, not separate entities. Blue Sky sits outside that boundary. See [handbook/company-facts.md](../../handbook/company-facts.md) and [handbook/locks.md](../../handbook/locks.md).
7. **June and July 2026 are not closed** — see [handbook/seats/controller.md](../../handbook/seats/controller.md) and the [run-controller](../run-controller/SKILL.md) skill. Do not describe a bill as posted into a closed month, and do not close a month from this seat.
8. Before anything from this seat goes anywhere external — a vendor, a client, a buyer — run it through [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md) or the [last-gate-then-stop](../last-gate-then-stop/SKILL.md) skill, and stop.

## Never
- Never report a savings total. None is sourced, and an estimate is still invented.
- Never invent a live pull from Bench. There is no Bench connector.
- Never invent an invoice, an accounts-receivable figure, a vendor, a bill amount, or a ledger balance.
- Never report June or July 2026 as closed.
- Never fill KPI "Current" with a number.
- Never let Blue Sky touch the LLC books.
- Never restate the seat page or the [How money moves](https://app.notion.com/p/3c125e30d68b81b49524fe7bc9f65c81) Notion page here — link them, don't copy them.
- Never name a person into this seat. Not recorded means not recorded.
- Never send anything from this seat without Michael. No program GitHub. See [handbook/locks.md](../../handbook/locks.md).
