---
name: run-meetings
description: Point to the fixed Company OS meeting cadence (:08/:38, :13/:43, :23/:53, daily PA+COO triage) and the Notion home for what actually happens in each one — never invent a meeting, an attendee, or a new cadence slot. Use when asked to run, join, or check on a Platformology meeting, or "what meeting is next."
---

# Run meetings

Reused from: [tonone-ai/tonone](https://github.com/tonone-ai/tonone), `skills/keel-cadence/SKILL.md` (the meeting-definition table shape) — inverted here, because Platformology's cadence is already locked by Michael, not something this skill designs — and the "never duplicate the reference in the skill body" rule already used across every `run-*` skill in this repo: [narrative-io/narrative-skills-marketplace](https://github.com/narrative-io/narrative-skills-marketplace), `docs/authoring-skills.md`, and [dzhng/skills](https://github.com/dzhng/skills), `skills/authoring/write-skills/SKILL.md`.

## The gate

The [Company OS home](https://app.notion.com/p/3c025e30d68b81cdbad7fdf5912e3ca3) (Notion) is the single source of truth for what happens in each meeting — agenda, notes, decisions. This repo names the cadence and stops; it does not host or restate any of that.

## The cadence — existing only, do not add a slot

| Slot | What runs here |
|---|---|
| :08 / :38 | Recurring cadence slot — see [Company OS home](https://app.notion.com/p/3c025e30d68b81cdbad7fdf5912e3ca3) for the live agenda |
| :13 / :43 | Recurring cadence slot — see [Company OS home](https://app.notion.com/p/3c025e30d68b81cdbad7fdf5912e3ca3) for the live agenda |
| :23 / :53 | Recurring cadence slot — see [Company OS home](https://app.notion.com/p/3c025e30d68b81cdbad7fdf5912e3ca3) for the live agenda |
| Daily | PA + COO triage — the two seats in it run [run-pa](../run-pa/SKILL.md) and [run-coo](../run-coo/SKILL.md) |

This is the whole cadence. If a request doesn't match one of these four rows, it is not a scheduled Platformology meeting — check [handbook/locks.md](../../handbook/locks.md) before treating anything else as standing.

## Steps

1. Confirm the slot against the table above. If it doesn't match one of the four rows, stop — don't invent a fifth slot to accommodate the request.
2. Open [Company OS home](https://app.notion.com/p/3c025e30d68b81cdbad7fdf5912e3ca3) for that slot's live agenda and notes. This repo does not host them.
3. **Do not invent an attendee.** Who's actually in the room is Notion's record — this repo's people roster ([handbook/people.md](../../handbook/people.md)) is not complete enough to assume one, and guessing an attendee list is the same failure mode as guessing a client fact.
4. **Never send** a meeting invite, recap, or follow-up without Michael. See [handbook/locks.md](../../handbook/locks.md).
5. Before anything drawn from a meeting goes anywhere external, run it through [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md).

## Never

- Never invent a new meeting slot, cadence, or recurring sync beyond the four rows above.
- Never invent an attendee, a decision, or a note that isn't already recorded in Notion.
- Never send a meeting invite, recap, or follow-up without Michael.
- Never fold this skill into [run-do-this](../run-do-this/SKILL.md) or [run-always-on](../run-always-on/SKILL.md) — meetings, daily work, and the COO cycle are three separate pointers to three separate Notion truths; don't collapse them to save a click.
