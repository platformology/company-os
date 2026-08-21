# When a seat is fully built

This page is for the CTO. It is a check-off, not a script — and one of its six boxes cannot be ticked yet, on purpose.

Five of the boxes are true or false today, on this M1. The sixth, the seat model on the shared office hand, waits on Michael's go: **"No local LLM until Michael says go"** is the wording on [locks.md](../locks.md), and Phase 4 of the go packet is the only thing that lifts it. A seat with the first five is as built as a seat gets today, and that is not a shortfall — it is the lock working.

## The hand, named

The shared always-on office hand is **Gemma 4 26B 8-bit on this M1**. That is recorded 19 Aug 2026 via the CTO and restated 20 Aug on the build map; it is named on [runtime.md](../runtime.md) and [runtime-brain.md](../runtime-brain.md), which own the rest of the picture. Two lines beside it, so nobody reaches for the wrong one:

- **Llama 3.3 70B 4-bit on this M1** is the on-purpose pen. It is **not a second seat brain**, and no seat is built on it.
- **Flash 2-bit** is the M5, SmarterVoice only, and the M5 is parked. No seat goes near it.

**Status today: not installed.** The hand is named and is not on the machine. This page does not put it there and does not tell anyone else to, so it carries **no build command, no run command, no model tag, no context size, and no sampler setting**. Those are not recorded in this repo — they belong to the go packet behind Phase 4, and they stay named missing in [SOURCES.md](../../SOURCES.md) instead of being guessed here. A guessed tag is a wrong tag, and a run line written today is Phase 4 taken early, which is a broken lock rather than a head start.

**Seats are never rebuilt as local models.** That lock does not lift at go. Installing the shared hand at Phase 4 does not turn a seat into one: what changes per seat is the SYSTEM text — that seat's body file — and nothing else. One set of weights, twenty-three bodies.

## The five boxes you can check today

Walk one seat at a time. Say the seat out loud, then check:

- [ ] **Desk file** — `handbook/desks/<seat>.md` is on disk, same slug as the seat page. A person can sit down with it and run a pass without asking what to click.
- [ ] **Body** — `handbook/bodies/<seat>.md` is on disk. Same slug. This is the file you paste into Claude or read here on this Mac, and the file that would become the seat model's SYSTEM text after go.
- [ ] **Seat page** — `handbook/seats/<seat>.md` is on disk. If the body and the seat page disagree, the seat page wins. Do not edit the seat page to match the body. Name the disagreement in [CONFLICTS.md](CONFLICTS.md) and on the desk.
- [ ] **Run page** — the seat's `run-*` page is a folder in [skills/](../../skills/README.md), the one named in [seat-job-map.md](../seat-job-map.md). The folder existing here is not the same as it being installed on this Mac as a Grok workflow. That second check is the one below, and this repo cannot see it.
- [ ] **Grok Bot profile** — this seat already has its own Grok Bot teammate chat on the M1. That chat is the wire ([runtime-wiring.md](../runtime-wiring.md)). Open it. It should be this seat, pointed at this desk and this seat page, not a second copy of another seat. This repo cannot see the Mac, so you confirm it there, on the machine.

If any of those five is empty, the seat is not built. A desk file on its own is not a built seat.

## The sixth box, and why it stays empty

- [ ] **Seat model on the shared hand** — **not available before Michael's go.** Nothing on this page or in this repo makes it available early.

This box is written down so it is not mistaken for an oversight, and so nobody closes it by installing something. Before go, the honest state of every seat's sixth box is empty, and the correct response to "can we just do this one seat" is the lock and a stop: run [check-locks](../../skills/check-locks/SKILL.md), name the lock, stop.

After go, the shape is one model definition per seat, all of them pointing at the same shared weights: the base never changes, the SYSTEM text is that seat's body file, and the name is the seat's slug. That shape is written out once, on [bodies/README.md](../bodies/README.md). This page does not restate it, and neither page carries a command for it.

## The twenty-three slugs

One slug per seat, the same one on all three files — and, after go, the name a seat model would be built under. Same names as [README.md](README.md).

| Seat | Slug | Run page |
|---|---|---|
| PA | `pa` | [run-pa](../../skills/run-pa/SKILL.md) |
| COO | `coo` | [run-coo](../../skills/run-coo/SKILL.md) |
| CMO | `cmo` | [run-cmo](../../skills/run-cmo/SKILL.md) |
| Head of Content | `head-of-content` | [run-content](../../skills/run-content/SKILL.md) |
| Head of Demand | `head-of-demand` | [run-demand](../../skills/run-demand/SKILL.md) |
| CSO | `cso` | [run-cso](../../skills/run-cso/SKILL.md) |
| Head of Sales | `head-of-sales` | [run-sales](../../skills/run-sales/SKILL.md) |
| SDR | `sdr` | [run-sdr-seat](../../skills/run-sdr-seat/SKILL.md) |
| CFO | `cfo` | [run-cfo](../../skills/run-cfo/SKILL.md) |
| Controller | `controller` | [run-controller](../../skills/run-controller/SKILL.md) |
| Bookkeeper | `bookkeeper` | [run-bookkeeper](../../skills/run-bookkeeper/SKILL.md) |
| CTO | `cto` | [run-cto](../../skills/run-cto/SKILL.md) |
| Head of Engineering | `head-of-engineering` | [run-engineering](../../skills/run-engineering/SKILL.md) |
| Developer | `developer` | [run-developer](../../skills/run-developer/SKILL.md) |
| CCO | `cco` | [run-cco](../../skills/run-cco/SKILL.md) |
| Head of Author Success | `head-of-author-success` | [run-author-success](../../skills/run-author-success/SKILL.md) |
| Client Success | `client-success` | [run-client-success](../../skills/run-client-success/SKILL.md) |
| CHRO | `chro` | [run-chro](../../skills/run-chro/SKILL.md) |
| People Ops | `people-ops` | [run-people-ops](../../skills/run-people-ops/SKILL.md) |
| VP Campaigns | `vp-campaigns` | [run-vp-campaigns](../../skills/run-vp-campaigns/SKILL.md) |
| Campaign Coordinator | `campaign-coordinator` | [run-campaign-coordinator](../../skills/run-campaign-coordinator/SKILL.md) |
| VP Retreats | `vp-retreats` | [run-vp-retreats](../../skills/run-vp-retreats/SKILL.md) |
| Retreat Producer | `retreat-producer` | [run-retreat-producer](../../skills/run-retreat-producer/SKILL.md) |

Parked and unassigned seats still get the same boxes. Their desk is a refuse-work pack. Checking a box does not unpark Engineering or Developer, and it does not assign Demand, Sales, or SDR.

## Leftover-file slugs — UNASSIGNED

The twenty-three leftover-file seats now have desk, body, seat page, and `run-*` on disk. Checking those boxes does not staff them. No Grok Bot profile is recorded for them in this repo. The sixth box stays empty for the same lock as the charter seats. Packet: [leftover-packet.md](../leftover-packet.md).

| Seat | Slug | Run page |
|---|---|---|
| Book Strategist | `book-strategist` | [run-book-strategist](../../skills/run-book-strategist/SKILL.md) |
| Book Writer | `book-writer` | [run-book-writer](../../skills/run-book-writer/SKILL.md) |
| Book Conceptual Editor | `book-conceptual-editor` | [run-book-conceptual-editor](../../skills/run-book-conceptual-editor/SKILL.md) |
| Book Copy Writer | `book-copy-writer` | [run-book-copy-writer](../../skills/run-book-copy-writer/SKILL.md) |
| Book Technical Editor | `book-technical-editor` | [run-book-technical-editor](../../skills/run-book-technical-editor/SKILL.md) |
| Book Reader | `book-reader` | [run-book-reader](../../skills/run-book-reader/SKILL.md) |
| Copy Writer | `copy-writer` | [run-copy-writer](../../skills/run-copy-writer/SKILL.md) |
| Copy Editor | `copy-editor` | [run-copy-editor](../../skills/run-copy-editor/SKILL.md) |
| Sales Writer | `sales-writer` | [run-sales-writer](../../skills/run-sales-writer/SKILL.md) |
| Sales Editor | `sales-editor` | [run-sales-editor](../../skills/run-sales-editor/SKILL.md) |
| Strategist | `strategist` | [run-strategist](../../skills/run-strategist/SKILL.md) |
| Persona Architect | `persona-architect` | [run-persona-architect](../../skills/run-persona-architect/SKILL.md) |
| Junior Digital Designer | `junior-digital-designer` | [run-junior-digital-designer](../../skills/run-junior-digital-designer/SKILL.md) |
| Senior Digital Designer | `senior-digital-designer` | [run-senior-digital-designer](../../skills/run-senior-digital-designer/SKILL.md) |
| Junior Print Designer | `junior-print-designer` | [run-junior-print-designer](../../skills/run-junior-print-designer/SKILL.md) |
| Senior Print Designer | `senior-print-designer` | [run-senior-print-designer](../../skills/run-senior-print-designer/SKILL.md) |
| Pendulum Wiki | `pendulum-wiki` | [run-pendulum-wiki](../../skills/run-pendulum-wiki/SKILL.md) |
| PR / Media | `pr-media` | [run-pr-media](../../skills/run-pr-media/SKILL.md) |
| SEO Expert | `seo-expert` | [run-seo-expert](../../skills/run-seo-expert/SKILL.md) |
| Social Media Strategist | `social-media-strategist` | [run-social-media-strategist](../../skills/run-social-media-strategist/SKILL.md) |
| Social Account Expert | `social-account-expert` | [run-social-account-expert](../../skills/run-social-account-expert/SKILL.md) |
| Speaking — Associations | `speaking-associations` | [run-speaking-associations](../../skills/run-speaking-associations/SKILL.md) |
| Speaking — Universities | `speaking-universities` | [run-speaking-universities](../../skills/run-speaking-universities/SKILL.md) |

## What this page will not start

- No VMs. No GKE. No program GitHub. No send without Michael.
- **No local model**, and no instruction that tells someone else to install one — not Ollama, not weights, not a smaller version of the install to get ahead.
- No Head of Engineering or Developer work.
- No HubSpot, no Bench connector, no Apple Contacts, no sixth tool.
- No edit to [locks.md](../locks.md). Lifting a lock, or changing one, is Michael's — and [runtime-brain.md](../runtime-brain.md) already says the same thing this page does: the hand is named, it is not installed, and it waits on his go.

## Conflicts we found

[CONFLICTS.md](CONFLICTS.md) lists every place a body file disagreed with its seat page. The seat page wins. This check-off does not "fix" those by editing a seat page.
