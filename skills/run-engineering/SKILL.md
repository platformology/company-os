---
name: run-engineering
description: Point to the Head of Engineering seat page — the seat is parked, so this skill answers questions about it and refuses to start work from it. Use when someone asks about sites, the production stack, engineering work, the M5, a VM, a GKE cluster, a local LLM, or who owns tech at Platformology.
---

# Run engineering

Reused from: [athola/claude-night-market](https://github.com/athola/claude-night-market), `plugins/abstract/skills/skill-authoring/modules/advanced-patterns.md` — the Activation Gate shape ("If either condition fails, stop and tell the user this skill does not apply. Do not silently proceed."), and [blouargant/yoke](https://github.com/blouargant/yoke), `docs/skills.md` — the "Hard rules" list plus the closing one-line verdict (`ok | needs-attention | blocked`). The pointer discipline — link the source page, never restate it — is the same one the rest of `skills/` uses.

Attribution note: this change does not touch [SOURCES.md](../../SOURCES.md). The two repos above still need rows there; whoever next edits that file should add them.

## The gate — this seat is parked
[handbook/seats/head-of-engineering.md](../../handbook/seats/head-of-engineering.md) is the source of truth for this seat. This skill does not restate it — open it first.

The seat is **parked**. Parked is not "slow" or "unstaffed" — it means engineering work does not start here. If the ask is work, the answer is: parked, here's the lock, stop. Do not quietly proceed on a smaller version of the ask.

## What the seat owns, and what's blocked
The seat owns sites and whatever production stack exists. Both sit behind the parked locks, and every one of these is a hard stop:

- **M5** stays parked until the machine is physically in hand.
- **No local LLM.**
- **No VMs.**
- **No GKE.**
- **No program GitHub** — do not touch, clone, fork, or open PRs on the program repos named in [handbook/locks.md](../../handbook/locks.md). **Do not start work on those repos from this page**, in any form: no branch, no scope, no estimate, no "just looking."

## Named missing
- **The production stack is named missing.** It is not written down in this repo. If asked what the stack is, say it isn't recorded — do not name a host, a framework, a database, or a deploy target, and do not reconstruct one from the seat's purpose.
- **Who fills this seat is not recorded** — see [handbook/people.md](../../handbook/people.md).

## Not this seat
Dave / Lehi Drew is a **vendor** for tech, not the seat holder — see [handbook/people.md](../../handbook/people.md). A vendor relationship is not a filled seat: don't record him as the holder, and don't route a seat decision to him as though he held it.

## Steps
1. Open [handbook/seats/head-of-engineering.md](../../handbook/seats/head-of-engineering.md) before answering anything.
2. Decide which kind of ask this is:
   - **A question about the seat** — answer from the seat page, and only from it.
   - **A request to do engineering work** — the seat is parked. Say so, name the specific lock that blocks it, and stop.
3. If the ask needs the production stack, say it's named missing. Don't fill the gap.
4. If the ask needs a seat holder, say it's not recorded. Don't fill that gap either.
5. Anything that actually needs deciding goes up: [CTO](../../handbook/seats/cto.md), and then Michael. **Unparking is not this skill's call** — M5 stays parked until the machine is physically in hand, and changing a lock is Michael's decision. See [handbook/locks.md](../../handbook/locks.md).
6. Before anything drawn from this seat goes anywhere external, run it through [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md).

## Never
- Never start, scope, branch, or estimate work on a program repo from this page.
- Never name or guess the production stack.
- Never stand up a VM, a GKE cluster, or a local LLM, and never treat the M5 as available.
- Never record Dave / Lehi Drew — or anyone else — as the seat holder.
- Never unpark the seat, or soften a lock to let a request through.
- Never restate the seat page in this skill — link it, don't copy it.
- Never send anything from this seat without Michael. See [handbook/locks.md](../../handbook/locks.md).

## How to close
End with one line so the reader knows where it landed: **parked**, naming the lock that blocked it, or **answered from the seat page**. Nothing in between.
