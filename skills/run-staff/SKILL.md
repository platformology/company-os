---
name: run-staff
description: Answer "who works here" from handbook/people.md and the Grok Bot staff Notion page — never invent a Role, and never promote a name off the Team page into staff. Use whenever someone asks who a person is, who to talk to, or who is on the team.
---

# Run staff

Reused from: [JGalego/TeamAPI](https://github.com/JGalego/TeamAPI), `docs/spec/teamapi-extended-v1.md` (members are "optionally assigned to roles," and a role can be vacant — so a person record stays valid with no Role recorded), and [narrative-io/narrative-skills-marketplace](https://github.com/narrative-io/narrative-skills-marketplace), `docs/authoring-skills.md` ("never duplicate" the reference in the skill body).

## The gate
Two pages answer every staffing question, and this skill is neither of them:

- [handbook/people.md](../../handbook/people.md) — the checked-in roster: who is staff, who is a vendor, and which Roles are recorded as missing.
- [Grok Bot staff](https://app.notion.com/p/3c125e30d68b81dc9116e2e62b47f143) (Notion) — the live page.

Open both before answering. This repo does not restate either.

## Who counts as what
Three buckets, and a name only moves buckets when Michael says so.

| Bucket | Who | Detail lives in |
|---|---|---|
| Staff — humans | Jhana (**no Role recorded**), Bob (**no Role recorded**), Anthony C. Garcia (COO / Chief Persona Architect) | [handbook/people.md](../../handbook/people.md) |
| Vendors — not employees | Dave / Lehi Drew (tech), David McInnis (Cranberry Press) | [handbook/people.md](../../handbook/people.md) |
| Everyone else on the Team page | Past, a vendor, or unknown — **unknown until proven** | Nowhere yet. Say "not recorded." |

A name appearing on the Notion Team page is not evidence that the person is current staff. Treat it as unknown and ask.

## Steps
1. Open [handbook/people.md](../../handbook/people.md). If the name is in the Staff or Vendors table, answer from that row and stop.
2. If the name is on the [Grok Bot staff](https://app.notion.com/p/3c125e30d68b81dc9116e2e62b47f143) page but not in `people.md`, answer that the person is past, a vendor, or unknown — not that they are staff — and ask Michael.
3. If asked what Jhana or Bob does, answer that **no Role is recorded**. Assigning either a Role is an ask-Michael-first item — see [handbook/locks.md](../../handbook/locks.md).
4. If asked for a vendor's scope beyond what `people.md` records, say it is not recorded rather than filling it in.
5. Before any answer about a person goes anywhere external, run it through [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md).

## Never
- Never invent a Role, a title, a seat assignment, or a reporting line for anyone. Jhana's and Bob's Roles are named missing in [SOURCES.md](../../SOURCES.md); leave them missing.
- Never call a vendor an employee. Dave / Lehi Drew and David McInnis are vendors.
- Never promote a name off the Notion Team page into staff, or infer that a person is current because they appear there.
- Never restate `people.md` or the Grok Bot staff page here — link them, don't copy them.
- Never send anything about a person without Michael. No program GitHub. See [handbook/locks.md](../../handbook/locks.md).
