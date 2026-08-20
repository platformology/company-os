# When a seat is fully built on the M1

This page is for the CTO. It is a check-off, not a script. A seat is "fully built" when every box below is true for that seat. You are not installing a model, and you are not turning a seat into one. The office hand is already on this Mac.

Recorded 20 Aug 2026 — Michael: the local office hand is **`office-hand`** = Qwen3.8 27B Q8 (`qwen3.8:27b-q8_0`), thinking off. One shared hand, twenty-three names. Gemma 4 31B Q6 stays on disk as backup only. Do not pull Flash onto this M1. Do not pull Qwen 16-bit. The M1 is the office. Grok Bot stays the manager.

**Seats are never rebuilt as local models.** That lock does not lift. What changes per seat is the name you call and the body text it reads. The weights stay one file.

The lock page still reads as if no local model is here until Michael says go — see [locks.md](../locks.md) and the leftover on [bodies/README.md](../bodies/README.md). This page does not rewrite that lock. Changing it is Michael's call. Until he does, the lock page governs, and this check-off is only for the hand he already named.

## For one seat, all six must exist

Walk one seat at a time. Say the seat out loud, then check:

- [ ] **Desk file** — `handbook/desks/<seat>.md` is on disk, same slug as the seat page. A person can sit down with it and run a pass without asking what to click.
- [ ] **Body** — `handbook/bodies/<seat>.md` is on disk. Same slug. This is the file you paste into Claude, read on this Mac, or load as the SYSTEM of the seat's name.
- [ ] **Seat page** — `handbook/seats/<seat>.md` is on disk. If the body and the seat page disagree, the seat page wins. Do not edit the seat page to match the body. Name the disagreement in [CONFLICTS.md](CONFLICTS.md) and on the desk.
- [ ] **Run page** — the seat's `run-*` page is a folder in [skills/](../../skills/README.md), the one named in [seat-job-map.md](../seat-job-map.md). The folder existing here is not the same as it being installed on this Mac as a Grok workflow. That second check is below, and this repo cannot see it.
- [ ] **Qwen alias, FROM `office-hand`** — on the M1, `ollama run <alias> --think=false` starts that seat's name. The alias is `FROM office-hand`. It is not a second download. Thinking is off on the call (`--think=false`, or `"think": false` on an API call), not as a line that rebuilds the weights. Confirm with `ollama show <alias>` that FROM is `office-hand` (or the same `qwen3.8:27b-q8_0` weights `office-hand` already is). If FROM points at anything else, the alias is wrong — fix the FROM, do not pull another model.
- [ ] **Grok Bot profile** — this seat already has its own Grok Bot teammate chat on the M1. That chat is the wire ([runtime-wiring.md](../runtime-wiring.md)). Open it. It should be this seat, pointed at this desk and this seat page, not a second copy of another seat. This repo cannot see the Mac, so you confirm it here, on the machine.

If any box is empty, the seat is not fully built. A desk file alone is not a built seat. An alias that pulled its own weights is not a built seat — it is a lock break.

## The twenty-three aliases

Same names as [README.md](README.md). One shared FROM.

| Seat | Alias | Run page |
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

Parked and unassigned seats still get the six boxes. Their desk is a refuse-work pack. Building the alias does not unpark Engineering or Developer, and it does not assign Demand, Sales, or SDR.

## How to make one alias, if it is missing

On the M1, next to the model, not in this repo:

```
FROM office-hand
PARAMETER num_ctx 8192
SYSTEM """
...paste the entire contents of handbook/bodies/<seat>.md here...
"""
```

Then `ollama create <alias> -f ./Modelfile.<alias>` and `ollama run <alias> --think=false`. Copy the file for the next seat. Change the name and the SYSTEM paste. FROM never changes.

The longer recipe, including why thinking is a per-call flag, is on [bodies/README.md](../bodies/README.md). If that page still says `FROM qwen3.8:27b-q8_0`, that is the same weights `office-hand` already is. Prefer `FROM office-hand` so a missing alias cannot become a second download.

## What this page will not start

- No VMs. No GKE. No program GitHub. No send without Michael.
- No Head of Engineering or Developer work.
- No HubSpot, no Bench connector, no Apple Contacts, no sixth tool.
- No rewrite of [locks.md](../locks.md) or [runtime-brain.md](../runtime-brain.md). Those still name an older hand. Flag that leftover to Michael.

## Conflicts we found

[CONFLICTS.md](CONFLICTS.md) lists every place a body file disagrees with its seat page. The seat page wins. This build check does not "fix" those by editing the seat.
