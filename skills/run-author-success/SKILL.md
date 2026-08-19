---
name: run-author-success
description: Run the Head of Author Success seat — point at handbook/seats/head-of-author-success.md and hand the actual work to the author-support-reply and support-call-prep skills. Use when someone asks how an author's engagement is going, or who owns author outcomes.
---

# Run author success

Reused from: [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills), `business-growth/skills/customer-success-manager/SKILL.md` (we took its shape — one seat watching how engagements are actually going — and inverted its weighted health scores, churn-risk tiers, and expansion scoring into a refusal, the same inversion [campaign-lead-scoring](../campaign-lead-scoring/SKILL.md) makes for lead scores), and [jwbreunsbach/uncommon-cco-library](https://github.com/jwbreunsbach/uncommon-cco-library), `skills/cs-launch-enablement.md` (unambiguous own-it / escalate-it rules, and "flag for review" in place of a guess). Pointer-not-copy discipline from [narrative-io/narrative-skills-marketplace](https://github.com/narrative-io/narrative-skills-marketplace), `docs/authoring-skills.md`, and [dzhng/skills](https://github.com/dzhng/skills), `skills/authoring/write-skills/SKILL.md`. The first two are new to this repo and are not yet listed in [SOURCES.md](../../SOURCES.md).

## The gate
- [handbook/seats/head-of-author-success.md](../../handbook/seats/head-of-author-success.md) — the seat: purpose, what it owns, who it reports to, who reports in. This skill does not restate it.
- [If a client writes](https://app.notion.com/p/3c025e30d68b81ada7b7cbf1d50b0d9f) (Notion) — the FAQ, and per the seat page the **only** source anything drafted from this seat, or from [Client Success](../../handbook/seats/client-success.md) underneath it, can come from.
- [handbook/clients.md](../../handbook/clients.md) — the only place author status is checked. Never a folder name, never HubSpot (HubSpot is closed).

## Where the work actually happens
This skill routes; it does not write client-facing text.
- A client wrote in and a reply is needed → [author-support-reply](../author-support-reply/SKILL.md). Draft only, gated by the FAQ page.
- A call is coming up and a brief is needed → [support-call-prep](../support-call-prep/SKILL.md). Support, never a pitch, gaps flagged not guessed.
- Anything about to leave your hands → [last-gate-then-stop](../last-gate-then-stop/SKILL.md) and [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md).

Neither of those two skills is restated here. Open the skill and run it.

## The chain
This seat reports to [CCO](../../handbook/seats/cco.md) — Chief Customer Officer, run with [run-cco](../run-cco/SKILL.md). [Client Success](../../handbook/seats/client-success.md) reports into this seat and holds day-to-day client communication — run with [run-client-success](../run-client-success/SKILL.md). Day-to-day drafting is that seat's job, not this one's; this seat owns the outcome and the gate.

## Steps
1. Open [handbook/seats/head-of-author-success.md](../../handbook/seats/head-of-author-success.md) and confirm the request is about author outcomes. Campaign QA and retreat experience sit at [CCO](../../handbook/seats/cco.md); a live campaign's day-to-day sits with [Campaign Coordinator](../../handbook/seats/campaign-coordinator.md) under [VP Campaigns](../../handbook/seats/vp-campaigns.md) — run it with [run-campaign](../run-campaign/SKILL.md).
2. Pull status from [handbook/clients.md](../../handbook/clients.md). As of the 18 Aug 2026 extract: 1 Alumni, 67 Past, 0 Current, 0 Prospect. Hoffman is a question, not a Current client.
3. Open the [If a client writes](https://app.notion.com/p/3c025e30d68b81ada7b7cbf1d50b0d9f) FAQ page before any client-facing wording exists, and route to the matching skill above.
4. **Cornelia Choe, our 1 Alumni:** her Thu 20 Aug 2026, 11:00–11:30am America/Denver meeting is **support, not a pitch.** Two Zoom URLs are on file and unresolved — flag both to Michael; do not pick one. No offer, no price, no upsell goes anywhere near her.
5. Own it or escalate it, and say which: **own it** when the answer is routing to the right skill, reading status off `clients.md`, or naming a gap. **Escalate to Michael** when it needs a send, an open number, a status change, or a Zoom URL chosen.
6. If the FAQ page doesn't cover the question, the answer is not covered — say so and flag it, in the same words [author-support-reply](../author-support-reply/SKILL.md) uses: **"Not in the FAQ — flag for Michael before sending."**
7. Run the result through [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md) and then stop.

## No author-health score
The customer-success template this skill borrows its shape from computes weighted health scores, churn-risk tiers, and expansion opportunities per account. **None of that is imported.** There is no author-health score, no churn tier, and no expansion play written down anywhere in this repo, and there is no portfolio to score against — Current is 0 and the KPI "Current" stays empty by design (see [handbook/clients.md](../../handbook/clients.md)). "How is this author doing?" is answered from `clients.md` and the FAQ page in plain sentences, or answered "not recorded."

## Never
- Never send. Every reply, brief, or summary from this seat is a draft for Michael or a named human — see [handbook/locks.md](../../handbook/locks.md).
- Never restate the seat page, the FAQ page, or the two skills this one routes to.
- Never invent a health score, a churn tier, an offer, a price, or a revenue figure for an author.
- Never treat an Alumni or Past-client support touch as a sales opportunity.
- Never pick between the two unresolved Cornelia Choe Zoom URLs.
- Never check author status against a folder name or HubSpot.
- No program GitHub. See [handbook/locks.md](../../handbook/locks.md).
