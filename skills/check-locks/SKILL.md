---
name: check-locks
description: Check the locks before you act — point at handbook/locks.md, never restate it, and when a lock trips, name the lock in plain words and stop. Use when any seat is about to send, touch program GitHub, start work the machine locks forbid, invent a client, a number, a person, or a price, or fill in something this repo has already named as missing.
---

# Check locks

Reused from: [alelaguard/agentguards-plugins](https://github.com/alelaguard/agentguards-plugins), `claude/skills/guardrails/SKILL.md` (run the check *before* the action rather than after, and answer in one fixed shape when it blocks — kept, but rewritten as a sentence a person says out loud instead of a tool call), and [arthursilas-ai/agent-preflight](https://github.com/arthursilas-ai/agent-preflight), `README.md` ("VERDICT: BLOCKED — do not deploy until the above are resolved," and "every finding carries a fix, not just a complaint" — so a refusal here names where the ask goes next). Point-don't-copy shape from [narrative-io/narrative-skills-marketplace](https://github.com/narrative-io/narrative-skills-marketplace), `docs/authoring-skills.md`, and [dzhng/skills](https://github.com/dzhng/skills), `skills/authoring/write-skills/SKILL.md` — the same shape already used by [run-faq](../run-faq/SKILL.md) and [run-kpis](../run-kpis/SKILL.md).

## The lock page is the source. This page is not.

[handbook/locks.md](../../handbook/locks.md) is the list. This skill walks you to it and gets out of the way. It does not restate the locks, does not summarize them, and does not keep a second copy that could quietly drift out of date from the real one.

Only Michael changes that page. This skill cannot add a lock, lift one, soften one, or read one generously so a request fits.

## When to run this

Before the action, not after it. Any seat — human or bot — about to:

- **Send** anything to a client, a prospect, or the public.
- **Touch program GitHub** — clone, fork, branch, link, or open a PR against a program repo.
- **Start work the machine locks forbid**, move the office or Grok Bot off this Mac, or plan on a VM, a cluster, or a local model existing.
- **Invent** a client, a money figure, a person, or a price.
- **Fill a named missing** — a blank this repo has already written down as missing, in [SOURCES.md](../../SOURCES.md).

If you're unsure whether an ask is one of those five, treat it as one. Open the page.

## Steps

1. Open [handbook/locks.md](../../handbook/locks.md) and read the ask against it. Read the actual page — not your memory of it, and not the short list in the [README](../../README.md), which is a pointer too.
2. **On the Never list** — stop. Nothing clears it for being urgent, small, obvious, or already half-done. Say which lock stopped it (see below) and hand the ask to Michael.
3. **Under "Ask Michael first"** — ask him. Don't decide it and don't decide it provisionally.
4. **Not on the page at all** — then it isn't locked, and this skill does not invent a lock to cover it. Hand the ask to the skill that owns the job; find it in [handbook/seat-job-map.md](../../handbook/seat-job-map.md).
5. Whatever survives, run [last-gate-then-stop](../last-gate-then-stop/SKILL.md) before it ships, then stop.

## Say it like a person

One line, in plain words, the way [run-faq](../run-faq/SKILL.md) says "Not in the FAQ — flag for Michael before sending":

> **Locked: no send without Michael.** The draft is ready; it goes to him, not out. See handbook/locks.md.

Name the one lock that actually stopped the ask and where the ask goes next. Don't stack a second stamp, a severity, or a score on top of it — one honest sentence and a stop is the whole thing. Keep thread IDs, message IDs, and page IDs out of it; Anthony, Jhana, Bob, or the next PA has to read this.

## Never

- **Never send without Michael** — no client, prospect, or public message leaves your hands. See [handbook/locks.md](../../handbook/locks.md).
- **Never touch program GitHub** — `smarter-voice`, `styleguide-os`, `academic-research-platform`, `book-campaign-platform`, `persona-standalone-programs`, `tlpF-b01-research-engine`. Named here so you recognize them; this repo does not link them.
- **Work runs on this Mac.** Machine locks live on [handbook/locks.md](../../handbook/locks.md) — this page does not restate them. Never stand up a VM or a GKE cluster — those two stay locked. A local model is locked until Michael says go too, and then it is Phase 4; that trigger lives on the lock page, not here.
- **Never invent a client, a money figure, a person, or a price**, and never fill KPI Current — see [handbook/clients.md](../../handbook/clients.md), [handbook/how-money-moves.md](../../handbook/how-money-moves.md), and [handbook/offers.md](../../handbook/offers.md).
- **Never give Jhana or Bob a Role** — both are blank, and a vendor stays a vendor, not a seat holder. See [handbook/people.md](../../handbook/people.md).
- **Never answer past the FAQ** — the FAQ is the gate, and Cornelia Choe is Alumni: support, never a pitch. See [run-faq](../run-faq/SKILL.md) and [handbook/clients.md](../../handbook/clients.md).
- **Never put a public price on Platinum Major List**, and never collapse a "both" listing into one number — quote both. See [handbook/offers.md](../../handbook/offers.md) and [place-on-offer-ladder](../place-on-offer-ladder/SKILL.md).
- **Never invent a new lock**, and never reword an existing one to make an ask fit. Changing [handbook/locks.md](../../handbook/locks.md) is Michael's call.
