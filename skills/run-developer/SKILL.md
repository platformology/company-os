---
name: run-developer
description: Point to the Developer seat page — the seat is parked under the same locks as Head of Engineering, so this skill answers questions about it and refuses to start coding from it. Use when someone asks to write, ship, fix, or review code, or asks who the developer is at Platformology.
---

# Run developer

Reused from: [athola/claude-night-market](https://github.com/athola/claude-night-market), `plugins/abstract/skills/skill-authoring/modules/advanced-patterns.md` — the Activation Gate shape ("If either condition fails, stop and tell the user this skill does not apply. Do not silently proceed."), and [designgrappler/agent-skills](https://github.com/designgrappler/agent-skills), `skills/add-specialist/SKILL.md` — the Scope Lock shape: work only on what's declared, and for anything outside it, "Do NOT make the change," flag it instead. The pointer discipline — link the source page, never restate it — is the same one the rest of `skills/` uses.

Attribution note: this change does not touch [SOURCES.md](../../SOURCES.md). The two repos above still need rows there; whoever next edits that file should add them.

## The gate — this seat is parked
[handbook/seats/developer.md](../../handbook/seats/developer.md) is the source of truth for this seat. This skill does not restate it — open it first.

The seat is **parked**, under the same locks as [Head of Engineering](../../handbook/seats/head-of-engineering.md) (see [run-engineering](../run-engineering/SKILL.md)). The purpose of the seat is to write and maintain code *once there's a machine and a stack to write it on*. Neither exists yet, so no code starts here. Don't proceed on a smaller version of the ask.

## What's blocked
Every one of these is a hard stop:

- **No local LLM.**
- **No VMs.**
- **No GKE.**
- **No program GitHub** — do not touch, clone, fork, or open PRs on the program repos named in [handbook/locks.md](../../handbook/locks.md). **Do not start work on those repos from this page**, in any form: no branch, no commit, no scope, no estimate, no "just reading the code first."
- Machine locks live on [handbook/locks.md](../../handbook/locks.md). Work runs on this Mac.

Scope lock: if you spot a change that looks necessary, that is not permission to make it. Flag it and hand it up.

## Named missing
- **The production stack is named missing** — see [handbook/seats/head-of-engineering.md](../../handbook/seats/head-of-engineering.md). There is nothing recorded to build on or deploy to. Don't name a language, framework, host, or repo layout to fill the gap.
- **Who fills this seat is not recorded** — see [handbook/people.md](../../handbook/people.md). "The developer" is not a person in this repo.

## Not this seat
Dave / Lehi Drew is a **vendor** for tech, not the seat holder — see [handbook/people.md](../../handbook/people.md). If someone says "ask the developer," that is a vendor question for Michael to route, not a seat this repo can hand work to.

## Steps
1. Open [handbook/seats/developer.md](../../handbook/seats/developer.md) before answering anything.
2. Decide which kind of ask this is:
   - **A question about the seat** — answer from the seat page, and only from it.
   - **A request to write, ship, fix, or review code** — the seat is parked. Say so, name the specific lock that blocks it, and stop.
3. If the ask assumes a stack, machine, or repo, say what's actually missing: the machine lock (see [handbook/locks.md](../../handbook/locks.md)) and the production stack (named missing).
4. If the ask needs a seat holder, say it's not recorded.
5. Anything that actually needs deciding goes up: [Head of Engineering](../../handbook/seats/head-of-engineering.md) / [CTO](../../handbook/seats/cto.md), and then Michael. **Unparking is not this skill's call** — changing a lock is Michael's decision. See [handbook/locks.md](../../handbook/locks.md).
6. Before anything drawn from this seat goes anywhere external, run it through [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md).

## Never
- Never start work on a program repo from this page — no clone, no branch, no commit, no PR, no estimate.
- Never write, run, or ship code against a stack that isn't recorded.
- Never name or guess the production stack.
- Never stand up a VM, a GKE cluster, or a local LLM. Work runs on this Mac. Machine locks live on [handbook/locks.md](../../handbook/locks.md).
- Never record Dave / Lehi Drew — or anyone else — as the seat holder.
- Never unpark the seat, or soften a lock to let a request through.
- Never restate the seat page in this skill — link it, don't copy it.
- Never send anything from this seat without Michael. See [handbook/locks.md](../../handbook/locks.md).

## How to close
End with one line so the reader knows where it landed: **parked**, naming the lock that blocked it, or **answered from the seat page**. Nothing in between.
