---
name: author-support-reply
description: Draft, never send, a reply to a client message, gated strictly by the "If a client writes" FAQ page. Use whenever a client — especially Cornelia Choe — writes in and a reply needs drafting.
---

# Author a support reply

Reused from: [river-labs-inc/agents](https://github.com/river-labs-inc/agents), `customer-support-agent/system-prompt.md` (the FAQ-as-gate model — "the FAQ is the contract," READY TO SEND vs. DRAFT, "you never claim to have sent anything — the user does the sending"), and [0xranx/golembot](https://github.com/0xranx/golembot), `templates/customer-support/skills/faq-support/SKILL.md` (log what the FAQ doesn't cover instead of guessing at it).

## The gate
The [If a client writes](https://app.notion.com/p/3c025e30d68b81ada7b7cbf1d50b0d9f) Notion page is the FAQ. It is the only source you draft from — the same way [`handbook/offers.md`](../../handbook/offers.md) is the only source for prices.

## Steps
1. Read the client's message in full.
2. Open [If a client writes](https://app.notion.com/p/3c025e30d68b81ada7b7cbf1d50b0d9f) and find the matching entry.
3. **If the client is Cornelia Choe** — she is Alumni (The Leaders Alliance); this is support, not a pitch. Nothing you draft offers her a new deal, a price, or an upsell — see [`handbook/clients.md`](../../handbook/clients.md). If her message concerns the Thu 20 Aug 2026, 11:00–11:30am America/Denver meeting, do not pick between the two unresolved Zoom URLs — flag both to Michael instead of choosing one.
4. **Question maps cleanly to a FAQ entry** — draft the reply in that entry's language. Do not add a price, an offer, or a fact that isn't in the entry or in `handbook/`.
5. **Question is not covered by the FAQ** — still draft only, and put this line at the top: **"Not in the FAQ — flag for Michael before sending."**
6. You never send this yourself. This skill produces a draft only. Sending is Michael's call — see [`handbook/locks.md`](../../handbook/locks.md): no send without Michael.
7. Before handing the draft over, run it through [`reviews/last-gate-checklist.md`](../../reviews/last-gate-checklist.md) (or the [last-gate-then-stop](../last-gate-then-stop/SKILL.md) skill).

## Never
- Never send, post, or reply directly — draft only, every time.
- Never invent a client fact, price, or offer that isn't in `handbook/` or the Notion FAQ page.
- Never treat a Cornelia Choe support reply as a sales opportunity.
- Never pick between the two Cornelia Choe Zoom URLs.
