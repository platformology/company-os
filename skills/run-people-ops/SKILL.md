---
name: run-people-ops
description: Run the People Ops seat off handbook/seats/people-ops.md — keep the contractor roster and the Team roster honest. Vendors stay vendors, and Jhana and Bob keep no Role. Use when someone asks who works here, whether a name is staff or a vendor, or wants a roster field filled in.
---

# Run People Ops

Reused from: [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills), `business-operations/skills/vendor-management/SKILL.md` (vendor records come from the vendor's own source, "not invented"; the artifact is "an input to a human decision, not the decision itself"), and [JGalego/TeamAPI](https://github.com/JGalego/TeamAPI), `docs/spec/teamapi-extended-v1.md` (a seat is independent of, and can be vacant of, its holder).

## The gate
Two sources run this seat; this skill does not restate either:
- [handbook/seats/people-ops.md](../../handbook/seats/people-ops.md) — the seat, which reports to [CHRO](../../handbook/seats/chro.md).
- [Grok Bot staff](https://app.notion.com/p/3c125e30d68b81dc9116e2e62b47f143) (Notion) — the live staff page.

The roster of record is [handbook/people.md](../../handbook/people.md). Open it before answering anything about a person.

## Steps
1. **Contractor roster.** Two names, both **vendors, not employees**: Dave / Lehi Drew (tech, for Platformology) and David McInnis (Cranberry Press). Those two facts — what they do and who they're a vendor for — are the whole record. `people.md` shows a dash for David McInnis's "what they do"; leave it a dash.
2. **Don't dress a vendor record up.** No rate, no contract term, no start or end date, no scope of work, no SLA, no tier. None of it is sourced. If someone needs one, it comes from the vendor's own paperwork via Michael, not from this repo.
3. **Team honesty.** The staff list is three rows, and two of them say "not recorded": Jhana — **no Role recorded**; Bob — **no Role recorded**; Anthony C. Garcia — COO / Chief Persona Architect (public title). This seat does not invent a Role, and per [handbook/locks.md](../../handbook/locks.md) assigning one is an ask-Michael-first item. Jhana and Bob also get no page in [handbook/seats/](../../handbook/seats/README.md), on purpose.
4. **Seat holders vs seats.** A seat and the person in it are tracked separately, and a seat can be vacant. Every seat except COO reads "Not recorded" in [handbook/seats/README.md](../../handbook/seats/README.md). That's the honest state of the org chart, not a set of blanks to fill. Classification questions above the roster go to [CHRO](../../handbook/seats/chro.md) — run [run-chro](../run-chro/SKILL.md).
5. **Roster changes are Michael's, not this seat's.** Anything that would add a person, change a classification, or record a Role is a change to `people.md` — draft the question, don't make the edit.
6. Before anything drawn from the roster goes anywhere external, run it through [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md).

## Never
- Never reclassify Dave / Lehi Drew or David McInnis as staff, and never reclassify a staff member as a vendor.
- Never give Jhana or Bob a Role, a title, a seat page, or a scope. "No Role recorded" is the answer.
- Never add a name that isn't in [handbook/people.md](../../handbook/people.md), and never record a family relationship, a spouse, or a child for anyone on the roster — none is sourced.
- Never invent a rate, a contract term, a start date, or a tenure length for a vendor or a staff member.
- Never fill a "Not recorded" seat holder with a guess, including your own inference from who does the work.
- Never restate the Grok Bot staff page in this repo — link it, don't copy it.
- Never send anything from the roster without Michael. No program GitHub. See [handbook/locks.md](../../handbook/locks.md).
