---
name: run-chro
description: Run the CHRO seat off handbook/seats/chro.md — contractors, role charters, and capacity — without inventing a Role for Jhana or Bob or a headcount plan for a three-person roster. Use when someone asks who is on the team, how a person is classified, what a seat is accountable for, or whether there's capacity to take on more work.
---

# Run CHRO

Reused from: [microsoft/github-copilot-modernization](https://github.com/microsoft/github-copilot-modernization), `plugins/github-copilot-modernization/skills/team-charters/SKILL.md` (a charter is Mission + what the role owns + a Core Principle naming what the role must **not** do; "ownership boundaries are strict"); [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills), `business-operations/skills/capacity-planner/SKILL.md` ("if you only have averages, stop and pull the distribution — single-point demand estimates are the most expensive anti-pattern in ops"); and [mohitagw15856/pm-claude-skills](https://github.com/mohitagw15856/pm-claude-skills), `skills/role-redesign-for-ai/SKILL.md` ("do not write 'focus on higher-value work' without naming the work").

## The gate
Two sources run this seat; this skill does not restate either:
- [handbook/seats/chro.md](../../handbook/seats/chro.md) — the seat: purpose, what it owns, what's locked, what's missing.
- [Grok Bot staff](https://app.notion.com/p/3c125e30d68b81dc9116e2e62b47f143) (Notion) — the live staff page.

The roster as recorded in [handbook/people.md](../../handbook/people.md) is three people — Jhana (**no Role recorded**), Bob (**no Role recorded**), Anthony C. Garcia (COO / Chief Persona Architect, public title) — plus two named vendors who are not employees. Nobody else. Open all three pages before answering anything about the team.

## Steps
1. **Contractors.** Dave / Lehi Drew (tech) and David McInnis (Cranberry Press) are **vendors, not employees** — see [handbook/people.md](../../handbook/people.md). Their records come from their own paperwork, not from inference. Reclassifying either one as staff changes `people.md`, so it goes to Michael first. Day-to-day roster mechanics belong to [People Ops](../../handbook/seats/people-ops.md) — run [run-people-ops](../run-people-ops/SKILL.md) for that.
2. **Role charters.** The charters already exist, one per seat, in [handbook/seats/](../../handbook/seats/README.md). A charter is written for the **seat, not the holder** — a seat can be occupied, unassigned, or parked, and the charter reads the same either way. What a seat does *not* do is part of its charter, not an omission from it: [run-campaign](../run-campaign/SKILL.md) and [run-retreat](../run-retreat/SKILL.md) exist because two adjacent seats keep getting collapsed into one.
3. **Do not write a charter for Jhana or Bob.** Neither has a Role recorded, they intentionally have no seat page ([handbook/seats/README.md](../../handbook/seats/README.md) says so), and assigning them one is an **ask-Michael-first** item in [handbook/locks.md](../../handbook/locks.md). "No Role recorded" is the answer to give.
4. **Capacity.** There is no volume, queue, pipeline, or hours data in this repo, so there is no capacity model to run and no headcount plan to produce. The honest read is the one already on the seat page: with a roster this size the seat's daily scope is thin too, until headcount changes. Say that, and name what you'd need — real demand figures from Michael — instead of sizing the team off an average nobody recorded.
5. **Don't backfill the empty seats into a capacity answer.** [Head of Demand](../../handbook/seats/head-of-demand.md), [Head of Sales](../../handbook/seats/head-of-sales.md), and [SDR](../../handbook/seats/sdr.md) are unassigned with no work assigned. [Head of Engineering](../../handbook/seats/head-of-engineering.md) and [Developer](../../handbook/seats/developer.md) are parked behind the machine locks. Counting any of them as capacity invents both a person and their output.
6. Before anything drawn from this seat goes anywhere external, run it through [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md).

## Never
- Never assign Jhana or Bob a Role, a title, a seat, or a scope. Ask Michael — see [handbook/locks.md](../../handbook/locks.md).
- Never reclassify a vendor as an employee, or an employee as a vendor.
- Never add a person who isn't in [handbook/people.md](../../handbook/people.md), and never record a family relationship, a spouse, or a child for anyone on the roster — none is sourced.
- Never invent a headcount plan, a utilization figure, a ramp, an attrition rate, or a hiring sequence. None of the inputs exists here.
- Never record a seat holder to fill a blank. Only the COO is recorded; every other seat is "Not recorded," which is the answer.
- Never restate the Grok Bot staff page in this repo — link it, don't copy it.
- Never send anything from this seat without Michael. No program GitHub. See [handbook/locks.md](../../handbook/locks.md).
