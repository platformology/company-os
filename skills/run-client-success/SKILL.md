---
name: run-client-success
description: Run the Client Success seat — day-to-day client communication, gated by the "If a client writes" FAQ page, drafted and never sent. Use when a client writes in, a routine client touch is due, or someone asks who handles day-to-day client communication.
---

# Run client success

Reused from: [river-labs-inc/agents](https://github.com/river-labs-inc/agents), `customer-support-agent/system-prompt.md` (the FAQ is the contract; DRAFT vs. READY TO SEND; "you never claim to have sent anything — the user does the sending"), and [0xranx/golembot](https://github.com/0xranx/golembot), `templates/customer-support/skills/faq-support/SKILL.md` (log what the FAQ doesn't cover instead of guessing at it) — both already named in [SOURCES.md](../../SOURCES.md). The own-it / escalate-it split is from [jwbreunsbach/uncommon-cco-library](https://github.com/jwbreunsbach/uncommon-cco-library), `skills/cs-launch-enablement.md`, and the health-score machinery we refuse is from [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills), `business-growth/skills/customer-success-manager/SKILL.md`; those two are new to this repo and are not yet listed in `SOURCES.md`.

## The gate
The [If a client writes](https://app.notion.com/p/3c025e30d68b81ada7b7cbf1d50b0d9f) (Notion) page is the FAQ, and it is the gate. It is the only source a client-facing draft from this seat comes from — the same way [handbook/offers.md](../../handbook/offers.md) is the only source for a price. If the FAQ doesn't cover it, this seat does not answer it; it flags it.

The seat itself is [handbook/seats/client-success.md](../../handbook/seats/client-success.md) — purpose, what it owns, who it reports to. This skill does not restate that page.

## What this seat does
Day-to-day client communication: the routine, unglamorous back-and-forth with the people we've worked with. Reports to [Head of Author Success](../../handbook/seats/head-of-author-success.md) (run with [run-author-success](../run-author-success/SKILL.md)), which reports to [CCO](../../handbook/seats/cco.md) — Chief Customer Officer (run with [run-cco](../run-cco/SKILL.md)). Outcomes and QA belong to those seats; the daily message traffic belongs here.

## Steps
1. Open [handbook/seats/client-success.md](../../handbook/seats/client-success.md) and the [If a client writes](https://app.notion.com/p/3c025e30d68b81ada7b7cbf1d50b0d9f) FAQ page. The FAQ page comes before any wording exists.
2. Confirm who you're talking to against [handbook/clients.md](../../handbook/clients.md) — 1 Alumni, 67 Past, 0 Current, 0 Prospect as of the 18 Aug 2026 extract. Folder names are not clients, Hoffman is a question rather than a Current client, and HubSpot is closed.
3. Draft with [author-support-reply](../author-support-reply/SKILL.md). That skill is the drafting procedure; this one does not duplicate it.
4. Prepping a call instead of a reply? Use [support-call-prep](../support-call-prep/SKILL.md) — support brief, never a pitch.
5. **Cornelia Choe, our 1 Alumni (The Leaders Alliance):** her communication is **support, not a pitch**, and her Thu 20 Aug 2026, 11:00–11:30am America/Denver meeting is a support call. Two Zoom URLs are on file and **unresolved** — flag both to Michael and do not pick one. Nothing drafted for her carries an offer, a price, or an upsell.
6. Covered by the FAQ → draft in that entry's language, adding nothing that isn't in the entry or in `handbook/`. Not covered → still draft only, with this line at the top: **"Not in the FAQ — flag for Michael before sending."**
7. Own it or escalate it, and say which: **own it** when the FAQ covers the question and the draft stays inside it. **Escalate to Michael** when it needs a send, a number the ladder leaves open, a status change, or a Zoom URL chosen — see [handbook/locks.md](../../handbook/locks.md).
8. Run every draft through [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md), or the [last-gate-then-stop](../last-gate-then-stop/SKILL.md) skill, hand it to Michael or a named human, and stop.

## Never send
This seat drafts. It does not send, post, schedule, or reply directly, and it never says a message went out. Sending is Michael's call, every time — see [handbook/locks.md](../../handbook/locks.md).

## Never
- Never send, post, or reply directly — draft only, every time, and never claim anything was sent.
- Never answer outside the FAQ page. If it isn't there, flag it instead of filling it in.
- Never invent a client fact, an offer, a price, a revenue figure, or a health score — there is no health score in this repo, and the KPI "Current" stays 0 and empty by design (see [handbook/clients.md](../../handbook/clients.md)).
- Never turn a day-to-day touch with an Alumni or Past client into a pitch.
- Never pick between the two unresolved Cornelia Choe Zoom URLs.
- Never record a client as Current, Prospect, or otherwise off "question" status — that's Michael's call.
- No program GitHub. See [handbook/locks.md](../../handbook/locks.md).
