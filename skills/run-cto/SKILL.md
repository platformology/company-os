---
name: run-cto
description: Point to handbook/seats/cto.md — never restate it. Use when someone asks the CTO seat to pick or name a stack, stand up infrastructure, touch a program repo, start work the machine locks forbid, or treat the tech vendor as the seat holder.
---

# Run CTO

Reused from: [narrative-io/narrative-skills-marketplace](https://github.com/narrative-io/narrative-skills-marketplace), `docs/authoring-skills.md` ("never duplicate" the reference in the skill body), and [dzhng/skills](https://github.com/dzhng/skills), `skills/authoring/write-skills/SKILL.md` ("keep a single source of truth"). The seat-is-not-its-holder split is the [JGalego/TeamAPI](https://github.com/JGalego/TeamAPI) `docs/spec/teamapi-extended-v1.md` model already used across [handbook/seats/](../../handbook/seats/README.md).

## The gate
[handbook/seats/cto.md](../../handbook/seats/cto.md) is the single source of truth for what this seat owns — which today is deliberately almost nothing. This repo does not restate it here; open it before doing anything.

This is the seat where the hardest locks land. They live in [handbook/locks.md](../../handbook/locks.md). This page points at them; it does not soften them.

## Locked, on this seat specifically
- **No program GitHub.** Do not touch, clone, fork, or open PRs against `smarter-voice`, `styleguide-os`, `academic-research-platform`, `book-campaign-platform`, `persona-standalone-programs`, or `tlpF-b01-research-engine`.
- **No VMs.**
- **No GKE.**
- **No local LLM.**
- Machine locks live on [handbook/locks.md](../../handbook/locks.md). Work runs on this Mac.
- **No send without Michael.**

## Steps
1. Open [handbook/seats/cto.md](../../handbook/seats/cto.md), then [handbook/locks.md](../../handbook/locks.md).
2. Check the ask against the locked list above. If it's on that list, the answer is no — not "not yet," not a workaround, not a smaller version of the same thing. Hand it to Michael; he's the only one who changes a lock.
3. **The production stack is named missing** — not written down in this repo. If asked what Platformology runs on, say it isn't recorded. Don't name a host, a framework, a database, or a deployment target. See [SOURCES.md](../../SOURCES.md).
4. **Dave / Lehi Drew is a vendor for tech, not the seat holder** — see [handbook/people.md](../../handbook/people.md). A vendor relationship is not a filled seat: don't answer "who's the CTO" with a vendor's name, and don't hand this seat's accountabilities to a vendor.
5. **Who fills this seat is not recorded.** That's the honest answer, not a placeholder for a guess — see [handbook/seats/README.md](../../handbook/seats/README.md).
6. The seats reporting in — [Head of Engineering](../../handbook/seats/head-of-engineering.md), and [Developer](../../handbook/seats/developer.md) under them — are parked under these same locks. Routing an ask down the chain doesn't unlock it.
7. Before anything drawn from this seat goes anywhere external, run it through [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md).

## Never
- Never restate [handbook/seats/cto.md](../../handbook/seats/cto.md) in this skill — link it, don't copy it.
- Never name a production stack, host, framework, or database for Platformology. It's named missing.
- Never treat Dave / Lehi Drew as the CTO or as this seat's holder.
- Never name who fills this seat.
- Never stand up a VM, a GKE cluster, or a local LLM — and never plan work that assumes one exists.
- Work runs on this Mac. Machine locks live on [handbook/locks.md](../../handbook/locks.md).
- Never start work on a program repo from this page, and never link one from this repo.
- Never lift or reword a lock to make an ask fit. Only Michael changes [handbook/locks.md](../../handbook/locks.md).
- Never send anything from this seat without Michael. See [handbook/locks.md](../../handbook/locks.md).
