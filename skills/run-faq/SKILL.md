---
name: run-faq
description: Point to the "If a client writes" FAQ page in Notion — never restate it — and hand any actual reply to the author-support-reply skill, which drafts and never sends. Use when a client message comes in and you need to know what the FAQ already answers.
---

# Run FAQ

Reused from: [river-labs-inc/agents](https://github.com/river-labs-inc/agents), `customer-support-agent/system-prompt.md` ("the FAQ is the contract," and a header a person can actually read — who wrote in, what they asked, which entry it matched — instead of a message ID), and [0xranx/golembot](https://github.com/0xranx/golembot), `templates/customer-support/skills/faq-support/SKILL.md` (log what the FAQ doesn't cover instead of reasoning past it). Point-don't-copy shape from [narrative-io/narrative-skills-marketplace](https://github.com/narrative-io/narrative-skills-marketplace), `docs/authoring-skills.md`, and [dzhng/skills](https://github.com/dzhng/skills), `skills/authoring/write-skills/SKILL.md`.

## The gate
[If a client writes](https://app.notion.com/p/3c025e30d68b81ada7b7cbf1d50b0d9f) (Notion) is the FAQ, and the FAQ is the gate. That page is live; this repo does not restate it — open it before you answer anything.

Nothing clears the gate for being obvious, urgent, or friendly. Either the FAQ covers the question, or it goes to Michael.

## Where this skill stops
This skill tells you what the FAQ covers. It does not write the reply. The moment a reply is needed, run [author-support-reply](../author-support-reply/SKILL.md) — that skill drafts, and only drafts. See [handbook/locks.md](../../handbook/locks.md): no send without Michael.

## Steps
1. Read the client's message in full, then open the FAQ and find the entry that matches it.
2. **Covered by the FAQ** — hand off to [author-support-reply](../author-support-reply/SKILL.md) and stay in that entry's language. Nothing gets added that isn't in the entry or in [`handbook/`](../../handbook/README.md).
3. **Not covered** — say so in those words: **"Not in the FAQ — flag for Michael before sending."** Write down what the FAQ failed to answer so the page can be fixed. Do not reason your way to an answer the page doesn't hold.
4. **Cornelia Choe is Alumni** (The Leaders Alliance) — this is support, not a pitch. Nothing drafted for her carries a new deal, a price, or an upsell; see [handbook/clients.md](../../handbook/clients.md). Her Thu 20 Aug 2026, 11:00–11:30am America/Denver meeting has two unresolved Zoom URLs — flag both to Michael rather than picking one.
5. Quote prices only from [handbook/offers.md](../../handbook/offers.md).
6. Before anything leaves your hands, run it through [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md).

## Keep the page readable
A person reads this — Anthony, Jhana, Bob, the next PA. So when you point at a client message:
- Name it the way a person recognizes it: who wrote in, what they asked, and when.
- Keep thread IDs, message IDs, Notion page IDs, and database row IDs out of the body. The link carries the ID; the words carry the name.
- Link the FAQ by its title, "If a client writes."

## Never
- Never restate the FAQ page in this repo — link it, don't copy it.
- Never send. This skill says what the FAQ covers, `author-support-reply` drafts, Michael sends. See [handbook/locks.md](../../handbook/locks.md).
- Never answer past the FAQ — an uncovered question gets flagged, not guessed.
- Never treat a Cornelia Choe message as a sales opening.
- Never pick between the two Cornelia Choe Zoom URLs.
- Never dump thread IDs or raw page IDs onto a page a person has to use.
- Never quote a price not on [handbook/offers.md](../../handbook/offers.md).
