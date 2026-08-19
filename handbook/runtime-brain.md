# Runtime brain

**Nothing on this page asks you to install anything. Today the answer is: don't.**

## The one-sentence version

The "brain" is one shared local model on the office Mac — and until Michael says go, it is not installed, so every seat keeps running exactly the way it runs now, on the Grok seat it already has.

## What "brain" means here

A brain — Michael's word for it is a **local hand** — is the model that does the thinking on the machine sitting in this office, so a seat can work the cheap hours without spending Grok tokens all day long.

**One hand, shared.** There are 23 seats in [seat-job-map.md](seat-job-map.md). There is not one model per seat, and there will not be 23 of them. A seat is a job plus a skill, not a model; the model is the hand a seat borrows when it needs one. Do not rebuild a seat as its own local model, and do not hand any seat a model of its own.

## Today: the hand is named missing as an install

- **No local LLM.** Do not install Ollama. Do not install any model. Do not tell Michael, a new hire, or another seat to install one. See [locks.md](locks.md).
- The hand is **named missing as an install** — named, because we know which one it is; missing, because it is not on the machine; and it stays missing until Michael says go.
- **Nothing changes in the meantime.** Every seat runs on its existing Grok seat, opens the skill in its row on [seat-job-map.md](seat-job-map.md), and follows [cheap-loop.md](cheap-loop.md).
- **The M1 is the office**, Daily Grok Bot lives on it, and the wake times stay 8am, then 11, 2, and 5. No hourly Grok wakes are added to cover anything on this page.

If you are new here and someone points you at this page: there is nothing for you to install, download, or set up. Reading it is the whole job.

## The slots

| Slot | What fills it | Which machine | Status today |
|---|---|---|---|
| The one shared hand the seats would use | Gemma | This M1 — the office | **Not installed.** Named for after go, and only after go |
| A second hand, SmarterVoice only | Flash | The M5 — the shop | **Parked.** Not a Platformology seat brain — Platformology is not SmarterVoice, see [company-facts.md](company-facts.md) |
| What every seat actually thinks with right now | Its existing Grok seat, plus the skill in its row | This M1 | **Running.** Unchanged by this page |

Three rows is the whole runtime. There is no fourth slot to fill in, and no row here is a placeholder waiting on someone's judgment.

## After Michael says go

The sequence is already locked, in four phases, in this order: clone this M1 onto the M5, the CTO proves the copy, strip this M1 to the office, and only then are models installed. **This page does not restate that packet.** The live source is Notion — [Desk](https://app.notion.com/p/3c125e30d68b81319e5bd9907af3d65e) for which machine is the office, and [When you say go](https://app.notion.com/p/3c125e30d68b81a3b351c0ce17aa4602) for what unparking the M5 actually means. In this repo it is locked on [locks.md](locks.md).

What that means for the brain, and nothing more than this:

- **Gemma on this M1 is the one named hand**, and putting it there is the fourth phase — the CTO's work, on Michael's go. It is not a new hire's job and it is not today's job.
- **The office does not move.** After the strip, this M1 is still the office, and Daily Grok Bot still lives on it.
- **The token rule does not change.** 8am, then 11, 2, and 5, with no hourly Grok wakes. The local hand covers the hours in between; it does not replace the wakes and it does not add any.
- **Grok still last-gates.** The cheap hours run local; anything on its way out still goes through [reviews/last-gate-checklist.md](../reviews/last-gate-checklist.md) first.

## Done-check

**Now, before go.** This page has done its job when:

1. it names the lock and names the hand,
2. nobody installs anything, and
3. a person can read it and say out loud, "one shared local model, not installed, not today."

**After go.** The runtime is done when:

1. one local hand is running on this M1,
2. the seats use it for the cheap hours, and
3. Grok still last-gates before anything goes out.

There is no partial credit between those two lists. Half-installed is not progress toward the second one — before go, it is a broken lock.

## Never

- Never install Ollama, a model, or anything that runs one, and never write an instruction that tells someone else to.
- Never give a seat its own model, and never rebuild a seat as a local model.
- Never treat the M5 as available, or plan any work that assumes the hand already exists.
- Never move Daily Grok Bot, or the office, onto the M5.
- Never add Grok wakes to cover an hour the local hand would have covered.
- Never unpark any of this yourself — changing a lock is Michael's call. Run [check-locks](../skills/check-locks/SKILL.md) first, name the lock, and stop.

## What this page is not

- **Not a plan.** No business, marketing, or R&D plan comes out of this page, and no client, dollar figure, person, or KPI figure goes into it. KPI Current stays empty.
- **Not an install guide, not a new stack, not a model architecture.** It is one page describing one slot on one machine.
- **Not a way to start parked work.** Demand, Sales, and SDR stay unassigned; Head of Engineering and Developer stay parked. See [seat-job-map.md](seat-job-map.md).

Every named gap in this repo is listed once in [SOURCES.md](../SOURCES.md). The hand is not one of them — it is not missing information, it is a locked decision, and the install waits on Michael.

## Reused shapes

Searched public GitHub before writing this page, per [reuse-what-github-has](../skills/reuse-what-github-has/SKILL.md):

- [cookys/autopilot](https://github.com/cookys/autopilot), `skills/dev-flow/references/model-routing.md` — one canonical file owns the slot table and every other page reads it rather than restating it, plus the line that the table "is a bootstrap preference, not a claim that every named model is currently qualified," which is exactly the gap between naming Gemma and installing it. Its dispatch tiers, escalation triggers, and benchmark evidence were left behind.
- [leestott/fl-mixedmodel](https://github.com/leestott/fl-mixedmodel), `README.md` — the cheap local path for ordinary work with the expensive path kept for the hard call, and "deterministic gates before LLM routing," since a lock is checked before anything runs and is never left to a model's judgment. Its confidence thresholds, fallback chains, and routing scores were left behind.
- Searched and **not** adapted: [ruvnet/agentic-flow](https://github.com/ruvnet/agentic-flow), `docs/guides/MULTI-MODEL-ROUTER.md`. It is a ten-provider router with budgets and failover — a stack, which is the opposite of one slot on one Mac, so nothing was taken.

Leftover: Index this file from handbook/runtime.md and README when that page lands.
