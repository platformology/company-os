# schemas/ — the five packet contracts

The intelligence layer's fixed shapes: what a seat is given, where the work is, what comes back, what gets handed on, and what gets recorded when a run refuses or breaks. Five schemas and this index, and nothing else in this folder.

Company: **Platformology LLC**. **Promote a Book** and **Book Retreat** are DBAs. Not SmarterVoice.

## The five schemas

| File | What it fixes | Visibility | Writer | Reviewer |
|---|---|---|---|---|
| [TASK_PACKET.schema.json](TASK_PACKET.schema.json) | The fixed input for one unit of seat work: role slug, named workflow, audience, requested outcome, source IDs, facts against assumptions against unknowns, constraints, allowed tools, prohibited actions, exact deliverables, acceptance criteria, approval points, stop conditions — and the locks the packet carries with it | Candidate-visible | Docs leftover | COO first QC, then PA last-gate |
| [TASK_STATE.schema.json](TASK_STATE.schema.json) | The in-flight state of one packet. Eight named states: `received`, `sourced`, `blocked`, `refused`, `drafted`, `repaired`, `verified`, `handed_off` | Candidate-visible | Docs leftover | COO first QC, then PA last-gate |
| [RESULT_PACKET.schema.json](RESULT_PACKET.schema.json) | The fixed output. "Not sourced" is a first-class valid result, and every claim carries one of PROVEN, SELF-REPORTED, UNVERIFIED, FAILED | Candidate-visible | Docs leftover | COO first QC, then PA last-gate |
| [HANDOFF_PACKET.schema.json](HANDOFF_PACKET.schema.json) | One seat-to-seat handoff: sender, receiver, and what is still unresolved | Candidate-visible | Docs leftover | COO first QC, then PA last-gate |
| [FAILURE_RECORD.schema.json](FAILURE_RECORD.schema.json) | One record per refusal, failure, or blocked run, on the twelve named failure classes | Candidate-visible | Docs leftover | COO first QC, then PA last-gate |
| [README.md](README.md) | This index | Candidate-visible | Docs leftover | COO first QC, then PA last-gate |

**Every file in this folder is candidate-visible.** No evaluator-only material lives here — not a fixture, not a trap, not a hidden acceptance file, and not a path to one. That separation is the reason this folder can be handed over whole.

**Who writes these.** The docs leftover writer, in GitHub, as a docs pull request. A Grok seat scopes, assigns, and first-QCs a leftover file — it does not write one. COO is first QC and the PA last-gates.

## Examples

Two synthetic files under [examples/](examples/), each there to prove one thing and nothing more:

| File | What it proves |
|---|---|
| [examples/RESULT_PACKET.not-sourced.valid.example.json](examples/RESULT_PACKET.not-sourced.valid.example.json) | A well-formed result whose every sourced field reads `"not sourced"` **validates**. Not sourced is a result, not a failure |
| [examples/HANDOFF_PACKET.no-live-receiver.invalid.example.json](examples/HANDOFF_PACKET.no-live-receiver.invalid.example.json) | A handoff to `sdr` **fails validation** on the receiver, and on nothing else. `developer` and `head-of-engineering` fail the same way |

Both are synthetic. No real client, author, employee, credential, price, or KPI figure appears in either; the identifiers and dates are placeholders.

## What the schemas encode

These are the rules already recorded elsewhere in this repo, written where a validator can reach them. Nothing below is a new rule.

- **No send without Michael.** `TASK_PACKET` carries `locks.send_requires_michael`, which can only be `true`, and an `external_send` block where declaring a send in scope forces Michael's sign-off to `required`. `RESULT_PACKET.send_performed` can only be `false` — a result cannot report a send.
- **No invented holder.** The only holder recorded anywhere is **COO — Anthony C. Garcia**, and the schemas will accept that name only on the `coo` slug. Every other seat reads `null`, which means not recorded. It does not mean vacant-and-fillable here.
- **KPI Current stays empty.** `locks.kpi_current` is an array with `maxItems: 0`. Empty is not 0, so a packet cannot carry a current value of any kind — including 0.
- **The two parked seats stay parked.** A `TASK_PACKET` for `head-of-engineering` or `developer` that asks for live job work is invalid, and `activation.activates_seat` can only be `false` on any packet at all. A `HANDOFF_PACKET` naming either as receiver is rejected.
- **The three leftover-only seats have no live job.** Same treatment for `head-of-demand`, `head-of-sales`, and `sdr`: no live job work in a packet, and rejected as a handoff receiver.
- **The definition gate holds.** What **CSO**, **CCO**, and **Pendulum** mean is not recorded. A packet for `cso`, `cco`, or `pendulum-wiki` must set `locks.definition_gate.applies` to `true`, must carry `seat-definition-not-recorded` among its unknowns, and can never declare the definition recorded. The gate travels with the work instead of being quietly resolved.
- **The gate chain travels too.** Approvals and handoffs name only **COO**, **PA**, or **Michael**. No other holder is recorded, so no other can be named. A `TASK_PACKET` must carry both a COO gate and a PA gate.
- **Nothing gets silently dropped.** `TASK_STATE` has eight states and a closed object, so a ninth cannot be added at the instance. Every state names the prior state it was reached from, `received` is the only entry, and `handed_off` appears in no predecessor list, which is what makes it terminal. A run that is `blocked` or `refused` must name a `FAILURE_RECORD` and an owner; a run that is `handed_off` must name the handoff.
- **Absence is never a pass.** There is no PASS label anywhere in these files. A claim whose evidence kind is `"not sourced"` can only be UNVERIFIED or FAILED, and a PROVEN claim must name evidence a reviewer can open or re-run. A field that was not sourced says so in its own value and may not carry a source it does not have; a deliverable that was not produced is reported with a reason rather than omitted.
- **A refusal and a breakage do not read the same.** `FAILURE_RECORD.kind` separates `refusal_on_lock`, `run_failure`, and `blocked_run`. A refusal must cite the lock it refused on; a run failure may not cite one. Refusing on a lock is correct behaviour, and the record says so rather than filing it as a defect.

## How these files are built

- **JSON Schema 2020-12.** No JSON Schema draft was in use anywhere in this repo before this folder — there were no `.json` files and no validator — so the current draft was taken.
- **Self-contained, on purpose.** No schema references another. Each carries its own `$defs`, including its own copy of the 46 seat slugs. That repeats the roster five times, and the trade is deliberate: any one file can be read or checked on its own, with no resolver, no bundler, and nothing fetched over a network. If the roster changes, all five change together.
- **No dependencies.** Nothing here adds an npm, GitHub, or ClawHub dependency, and nothing was cloned.

## How to check them

There is no validator in this repo, and adding one was out of scope for this unit. Two levels:

1. **Parse.** `python3 -c "import json; json.load(open(f))"` on each of the five files. Stdlib only.
2. **Validate.** Any JSON Schema 2020-12 validator, run offline against the two files in `examples/`. The first must pass and the second must fail on the receiver. Both files are in the repo, so a reviewer can re-run this rather than take it on report.

The run behind this pull request was done that way, with a throwaway stdlib checker that was not committed: the five files parse, the not-sourced example validates, and the `sdr` handoff fails on the receiver rule and on nothing else. **That recorded run is SELF-REPORTED** — no artifact hash was minted for it. What is **PROVEN** is that the files are openable paths in this repo, so anyone can reproduce the result instead of believing it.

## What this folder does not do

It does not activate anyone, staff a seat, unpark a seat, or create a live job. It installs nothing. It invents no company fact, holder, client, price, pipeline, KPI figure, or legal, accounting, or HR rule. It holds no `recipes/`, `routing/`, `knowledge/`, or evaluator-only material, and it does not restate the Phase 0 report.

Named gaps stay named. Full list: [SOURCES.md](../../../../SOURCES.md).
