---
name: place-on-offer-ladder
description: Look up the public price for a Platformology offer and quote it correctly, including quoting both numbers when the ladder shows two, or saying "no public price" / "named missing" when that's the honest answer. Use whenever anyone asks what an offer costs, or asks for a price to be put into a draft.
---

# Place on the offer ladder

Reused from: [dswh/company-os](https://github.com/dswh/company-os), `brain/offers.md` (the "never quote a price not written here" rule), and the open Agent Skills `SKILL.md` frontmatter convention documented at [ItamarZand88/awesome-agent-conventions](https://github.com/ItamarZand88/awesome-agent-conventions/tree/main/conventions/skill-md) (name + description as the activation trigger, procedural body).

## When to use this
A client, a bot, or a new hire asks what an offer costs, or asks you to put a number into a message.

## Steps
1. Open [`handbook/offers.md`](../../handbook/offers.md). That table is the only source of public prices — not memory, not a guess, not last quarter's deck.
2. Find the offer's row.
3. **One price listed** — quote it exactly as written.
4. **"X or Y" listed** — quote both numbers, in that order. Do not average them, and don't pick the lower one to look cheap or the higher one to look premium.
5. **"No public price" (Platinum Major List)** — say exactly that. Do not invent one.
6. **Lead magnet** — there is no Offers row for it. Say "no listed price," don't borrow the nearest tier's number.
7. **Membership** — the price is named missing (see [`SOURCES.md`](../../SOURCES.md)). Say "price not published, check with Michael" — don't estimate from a comparable tier.
8. Before this goes anywhere external, run [`reviews/last-gate-checklist.md`](../../reviews/last-gate-checklist.md).

## Examples
> Ask: "What does Professional cost?"
> Answer: "$20,000, per the current public offer ladder."

> Ask: "What does Multi-author cost?"
> Answer: "Publicly quoted both ways — $1,000 or $20,000. I can't collapse that to one number; check with Michael on which applies here."

> Ask: "What's the membership price?"
> Answer: "Not published. Named missing — check with Michael before quoting anything."

## Never
- Never invent a price, a discount, a bundle, or a "starting at" figure not on the ladder in `handbook/offers.md`.
- Never resolve a "both" listing into a single number on your own authority.
- Never send a price to a client — quoting and drafting are not the same as sending. See [`handbook/locks.md`](../../handbook/locks.md): no send without Michael.
