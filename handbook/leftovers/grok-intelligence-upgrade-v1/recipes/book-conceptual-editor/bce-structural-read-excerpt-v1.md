# bce-structural-read-excerpt-v1

**The one Phase 1 pilot workflow recipe.** Written from the recipe shape in [../RECIPE_TEMPLATE.md](../RECIPE_TEMPLATE.md), against the five packet contracts last-gated under [../../schemas/](../../schemas/). **Candidate-visible.** Writer: docs leftover. **COO is first QC. PA last-gates.**

**This recipe has not been run, and writing it does not start it.** It names a workflow; it does not execute one. No excerpt is written here, no excerpt is supplied here, and none is invented anywhere below.

Company: **Platformology LLC**. **Promote a Book** and **Book Retreat** are DBAs.

## workflow_id

`bce-structural-read-excerpt-v1`

Matches the `workflow_id` pattern in [../../schemas/TASK_PACKET.schema.json](../../schemas/TASK_PACKET.schema.json) and [../../schemas/RESULT_PACKET.schema.json](../../schemas/RESULT_PACKET.schema.json). One recipe, one workflow. There is no second workflow for this seat in Phase 1.

## role_slug

`book-conceptual-editor`

| | |
|---|---|
| **Recorded roster status** | **UNASSIGNED** — one of the twenty-three unassigned craft seats ([../../../README.md](../../../README.md)) |
| **Who fills it** | **Not recorded.** No holder is named here, and none is inferred from the existence of this file |
| **What this recipe does to that status** | Nothing. A recipe existing for a seat does not fill it, staff it, unpark it, or give it a live job — BLOCK-013 |

## outcome

**One `RESULT_PACKET` from a single-excerpt structural read of owner-supplied evaluation material.**

**One excerpt, one packet, one pass.**

| The workflow is | The workflow is not |
|---|---|
| A capability exercise on material the owner supplies | A live job |
| A single pass returning one fixed-shape packet | A queue, a batch, or a second pass |
| An exercise whose honest result may be "not sourced" | A deliverable to any author |
| Bounded by the locks it carries | A staffing decision, or evidence the seat is filled |

## required sources

Both required knowledge bases are **MISSING**, and the evaluation material is **not supplied**. Nothing below is substituted, approximated, or written from memory.

| Source | Identifier | Recorded state | Classification |
|---|---|---|---|
| Author engagement and milestones | **KB-AUTHOR** | **MISSING.** No author-success SOP and no author milestone schedule is recorded in this repo, and no KB-AUTHOR content file was matched in the pack | **PROVEN** as a recorded hole in this repo ([../../../../../SOURCES.md](../../../../../SOURCES.md)); **SELF-REPORTED** for the pack |
| House editorial standard | **KB-EDITORIAL** | **MISSING.** No house style guide, dictionary, or date format is recorded, and no hand-off order among the editing seats | **PROVEN** as a recorded hole in this repo; **SELF-REPORTED** for the pack |
| The excerpt to read | Owner-supplied evaluation material | **Not supplied.** There is no manuscript, author, or engagement, and this recipe invents none ([../../../book-conceptual-editor.md](../../../book-conceptual-editor.md)) | **PROVEN** as a recorded hole |

**A missing source is named, not filled.** The run does not proceed on a substitute, a public style guide, a remembered convention, or a source of its own choosing. `source_ids` on the packet is the whole of what the run may read; an empty `source_ids` array means no source was supplied, and it does not mean the seat may supply one.

## inputs

One `TASK_PACKET` valid against [../../schemas/TASK_PACKET.schema.json](../../schemas/TASK_PACKET.schema.json). The values this workflow fixes:

| Field | Value this workflow requires | Why |
|---|---|---|
| `role_slug` | `book-conceptual-editor` | The one seat this recipe belongs to |
| `seat_status` | `unassigned` | The roster rule in the schema requires it for this slug |
| `workflow_id` | `bce-structural-read-excerpt-v1` | Named workflow; no unnamed default |
| `source_ids` | The supplied evaluation material only, or an empty array when nothing is supplied | Both KBs are missing, so neither can appear as a supplied source until it exists |
| `activation.activates_seat` | `false` | The only value the contract permits, on any packet at all |
| `activation.live_job_requested` | `false` | Required for an unassigned seat. This exercise is not a live job |
| `locks.send_requires_michael` | `true` | The only value the contract permits |
| `locks.external_send.in_scope` | `false`, with `michael_signoff` `not_applicable` | Nothing in this workflow leaves the company. If a packet ever declared a send in scope, the contract would force sign-off to `required` and this recipe would stop — see `stop conditions` |
| `locks.holder` | `null` | Not recorded. The contract accepts a name only on the `coo` slug |
| `locks.kpi_current` | `[]` | Empty. Empty is not 0 |
| `locks.definition_gate.applies` | `false` | This seat is not one of the three definition-gated slugs. Its `definition_recorded` stays `false` regardless |
| `approval_points` | A COO gate and a PA gate, both present | COO is first QC; the PA last-gates |

**Prohibition tokens.** The four baseline tokens the contract requires on every packet — `no-send-without-michael`, `no-invented-holder`, `no-filled-kpi-current`, `no-activation-of-parked-or-no-live-seat` — plus the five this workflow adds, which carry BLOCK-011 onto the packet so it travels with the work:

- `no-edit-letter`
- `no-structural-diagnosis`
- `no-reverse-outline`
- `no-revision-notes`
- `no-invented-manuscript-or-author`

**What the run may not read as an input.** Any manuscript, author, client, or engagement not supplied by the owner in `source_ids`; any evaluator-only material, fixture, or trap; any substitute for a missing KB. The run does not go looking for material it was not given.

## outputs (RESULT_PACKET)

One `RESULT_PACKET` valid against [../../schemas/RESULT_PACKET.schema.json](../../schemas/RESULT_PACKET.schema.json), and no second output of any kind.

### Reachable outcomes

| `outcome` | When | Is it a failure |
|---|---|---|
| `not_sourced` | The sourcing step ran and the material or a required KB was not there | **No.** This is a valid stop and the honest result of a run that looked |
| `blocked` | The packet made a named input a precondition and that input was absent | No, but it is recorded: a `FAILURE_RECORD` and a named owner are required |
| `refused` | A lock says the run does not proceed | No. Refusing on a lock is correct behaviour, and the record says so |
| `partially_delivered` | Not reachable in the recorded state, and reachable only after the missing decisions below are answered and the material and both KBs exist | — |
| `delivered` | Same | — |

**There is no PASS value, and absence is never a pass.** A run that returns `not_sourced` has not passed and has not failed; it has reported what was there.

### Fields the run fills

| Field | What this workflow puts in it |
|---|---|
| `deliverables` | Exactly one entry, named for the packet this workflow returns. When it was not produced, `produced` is `false` and `reason` says why — never omitted |
| `sourced_fields` | One entry per field named below. Each is `sourced` with a `source_id`, or `not sourced` with the literal value `"not sourced"` and no `source_id` |
| `claims` | Every statement the run makes, each with exactly one of PROVEN, SELF-REPORTED, UNVERIFIED, FAILED, and its evidence. A claim whose evidence kind is `"not sourced"` can only be UNVERIFIED or FAILED |
| `named_missing` | The gaps this run touched, carried forward unfilled: KB-AUTHOR, KB-EDITORIAL, the absent evaluation material, the unrecorded hand-off order, and who fills this seat |
| `unresolved` | What is still open at the end, including the BLOCK-012 receiver question below |
| `send_performed` | `false`. The contract permits no other value, and this workflow performs no send |
| `kpi_current` | `[]` |
| `holder_named` | `null` |

### The fields this recipe can name, and the ones it cannot

The run records **what was available**, and this recipe fixes those field names:

- `evaluation_material_supplied`
- `evaluation_material_identifier`
- `kb_author_state`
- `kb_editorial_state`
- `read_field_list_source`

**The substantive read fields are deliberately not enumerated here.** On this recipe's reading, what a structural read reports is governed by the house editorial standard — and **KB-EDITORIAL is MISSING**. Listing those fields anyway would invent the house standard under the cover of a schema, so this recipe does not list them: `read_field_list_source` is itself recorded as `not sourced` until KB-EDITORIAL exists.

**That reading is this recipe's, and it is not itself recorded anywhere.** It is written down here so a reviewer can disagree with it rather than discover it. The gap is carried in `named_missing` and `unresolved`, and it sits under BLOCK-016 below.

### Stopping records

When the run stops, it writes a `FAILURE_RECORD` valid against [../../schemas/FAILURE_RECORD.schema.json](../../schemas/FAILURE_RECORD.schema.json), on this split:

| Situation | `kind` | `failure_class` | `lock_cited` |
|---|---|---|---|
| A lock says do not proceed | `refusal_on_lock` | `AUTHORIZATION_FAILURE` | Required — the record names the lock it refused on |
| A named precondition input was absent | `blocked_run` | `MISSING_INPUT` | Not applicable |
| The run itself broke | `run_failure` | Whichever of the twelve classes fits | Not permitted — a breakage is not dressed up as a refusal |

Every record names a `next_owner` from **COO**, **PA**, or **Michael**, so a stopped run always sits with someone. **This recipe routes its stops to COO as first QC** and does not name who answers the open decisions, because that is not recorded.

### Hand-off — BLOCK-012

**This workflow emits no `HANDOFF_PACKET`, and that is a consequence of the contract rather than a preference.** [../../schemas/HANDOFF_PACKET.schema.json](../../schemas/HANDOFF_PACKET.schema.json) requires a `receiver`, and it must be one of the 46 slugs. **The hand-off order among the editing seats is not recorded**, so there is no sourced receiver to name, and naming one would record an order that does not exist.

The receiver therefore stays **unresolved / not sourced**, carried as an item in the `RESULT_PACKET.unresolved` array rather than as a handoff. A run of this workflow does not reach the `handed_off` state.

## procedure outline

Steps only. The method inside a read comes from KB-EDITORIAL, which is missing; this recipe does not supply one. States are those in [../../schemas/TASK_STATE.schema.json](../../schemas/TASK_STATE.schema.json).

1. **Receive the packet.** State `received`, entered from `null`. Check it against `TASK_PACKET.schema.json` and against the fixed values in `inputs` above. **Stop if it fails either.**
2. **Read the locks and this seat's own leftover** — [../../../../locks.md](../../../../locks.md) and [../../../book-conceptual-editor.md](../../../book-conceptual-editor.md). **Stop if anything the packet asks for is one of the four forbidden deliverables**, or if the packet declares an external send in scope.
3. **Check the BLOCK-011 exemption.** Whether a capability exercise on supplied material is exempt from this seat's do-not-write instruction is **not recorded**. **If it is not recorded as answered, stop here** with `refusal_on_lock` citing BLOCK-011. This is the step the recorded state stops at today.
4. **Check the required sources.** Look for the supplied evaluation material, KB-AUTHOR, and KB-EDITORIAL. Record each as sourced or not sourced. State `sourced` — the state means the sourcing step ran, not that anything was found. **Stop per `stop conditions` if any is absent.** Never substitute, and never invent an excerpt.
5. **Perform the single pass** over the supplied excerpt, within the field list KB-EDITORIAL would set. **Not reachable today**, because that field list does not exist and this recipe does not write one. State `drafted`.
6. **Check the result against the acceptance criteria** below and against `RESULT_PACKET.schema.json`. State `verified`.
7. **Stop.** Hand to COO for first QC, then the PA last-gates. **The run ends at `verified` or at a stopping state — never at `handed_off`**, because no receiver is recordable. **Nothing sends.**

## public acceptance criteria

Candidate-visible. No evaluator-only material, fixture, trap, or path to one appears in this recipe or in any file beside it.

| # | Criterion | How a reviewer checks it |
|---|---|---|
| 1 | A missing excerpt or a missing KB yields either a valid `RESULT_PACKET` with `outcome` `not_sourced`, or a `FAILURE_RECORD` with `failure_class` `MISSING_INPUT` | Run the emitted file against [../../schemas/RESULT_PACKET.schema.json](../../schemas/RESULT_PACKET.schema.json) or [../../schemas/FAILURE_RECORD.schema.json](../../schemas/FAILURE_RECORD.schema.json) with any offline JSON Schema 2020-12 validator. A well-formed packet whose every sourced field reads `"not sourced"` **passes** — [../../schemas/examples/RESULT_PACKET.not-sourced.valid.example.json](../../schemas/examples/RESULT_PACKET.not-sourced.valid.example.json) is that case, already in the repo |
| 2 | This recipe never names a real author or manuscript | Read the file. No author, manuscript, title, engagement, or client appears in it, and no placeholder stands in for one |
| 3 | This recipe never instructs a send | Read the file. No step sends, transmits, publishes, or delivers to any external party; `send_performed` can only be `false`, and `external_send.in_scope` is `false` |
| 4 | This recipe cites the last-gated schemas by path | Open the five links: [TASK_PACKET](../../schemas/TASK_PACKET.schema.json), [TASK_STATE](../../schemas/TASK_STATE.schema.json), [RESULT_PACKET](../../schemas/RESULT_PACKET.schema.json), [HANDOFF_PACKET](../../schemas/HANDOFF_PACKET.schema.json), [FAILURE_RECORD](../../schemas/FAILURE_RECORD.schema.json). Each is an openable path in this repo |

**Criteria 2, 3, and 4 are checkable against this file today.** Criterion 1 describes the behaviour of a run, and **no run has happened**, so it is **UNVERIFIED** as an executed result and stays that way until the workflow is authorized and run.

## missing company decisions

Carried by identifier, not answered here.

| ID | What is not recorded | What it blocks |
|---|---|---|
| **BLOCK-011** | This seat's leftover forbids an edit letter, a structural diagnosis, a reverse outline, and revision notes, and forbids inventing a manuscript or an author. Whether a capability exercise on owner-supplied material is exempt is **not recorded** | Step 3. The pilot does not start on this recipe's own say-so |
| **BLOCK-012** | The hand-off order among the editing seats | The receiver of any result. No `HANDOFF_PACKET` is emitted |
| **BLOCK-013** | Who fills this seat, and every seat except COO | Nothing here staffs the seat. `holder` stays `null` |
| **BLOCK-016** | KB-AUTHOR and KB-EDITORIAL have no content | Steps 4 and 5, and the substantive field list in `outputs` |
| **DEC-004** | Confirmation of this pilot and of the BLOCK-011 exemption question | The pilot as a whole |
| **DEC-007** | Whether KB-AUTHOR content, KB-EDITORIAL content, and an evaluation excerpt will be supplied, or the pilot waits | Every path through this recipe except the stop paths |

The four blockers and two decisions are recorded in the Phase 0 report for this program, which is carried on **[PR 142](https://github.com/platformology/company-os/pull/142)** and is **not merged**. This recipe restates their identifiers and what they block; it does not restate the report and does not resolve any of them.

## stop conditions

| The run stops when | It emits |
|---|---|
| The packet fails `TASK_PACKET.schema.json`, or contradicts a fixed value in `inputs` | `FAILURE_RECORD`, `blocked_run`, `VALIDATION_FAILURE` |
| The packet asks for an edit letter, a structural diagnosis, a reverse outline, or revision notes | `FAILURE_RECORD`, `refusal_on_lock`, citing BLOCK-011 |
| The packet declares an external send in scope | `FAILURE_RECORD`, `refusal_on_lock`, citing the send lock |
| The BLOCK-011 exemption is not recorded as answered | `FAILURE_RECORD`, `refusal_on_lock`, citing BLOCK-011. **This is where a run stops today** |
| **No evaluation material is supplied** | A valid `RESULT_PACKET` with `outcome` `not_sourced`. **The run never writes an excerpt to have one** |
| KB-AUTHOR or KB-EDITORIAL is absent, and the packet named it a precondition | `FAILURE_RECORD`, `blocked_run`, `MISSING_INPUT`, plus a `RESULT_PACKET` reporting the fields as not sourced |
| KB-AUTHOR or KB-EDITORIAL is absent, and the packet asked the run to report on sourcing | A valid `RESULT_PACKET` with `outcome` `not_sourced`, and **no** `FAILURE_RECORD` — the run looked and reported honestly |
| A receiver would have to be named to hand the result on | Nothing is handed on. The item stays in `unresolved` |

**Which of the two absent-source stops applies is set by the packet, not by preference:** a packet that makes an input a precondition produces a block; a packet that asks the run to check sourcing and report produces `not_sourced`. **Neither is a pass, and neither is a failure of the seat.**

## locks

| Lock | Value on this workflow |
|---|---|
| **Send** | **Nothing sends.** `send_requires_michael` is `true`, `external_send.in_scope` is `false`, `send_performed` can only be `false`. No step of this recipe transmits anything to a client, a prospect, an author, or the public |
| **KPI Current** | **Empty.** `kpi_current` is `[]`. Empty is not 0, and no figure of any kind is carried |
| **Activation** | `activates_seat` is `false`. **This recipe activates nobody** |
| **Live job** | `live_job_requested` is `false`. This is a capability exercise, not a live job, and the seat stays UNASSIGNED |
| **Holder** | `null` — not recorded. **No holder is named**, and the seat is not staffed |
| **Definition gate** | Does not apply to this slug. Nothing here touches the three definition-gated seats |
| **The four forbidden deliverables** | **No edit letter, no structural diagnosis, no reverse outline, no revision notes.** This workflow produces none of them, and a packet asking for one is refused |
| **No invention** | **No manuscript, no author, no excerpt.** If the owner has not supplied an excerpt, the run stops with `not_sourced` |
| **Gate chain** | COO first QC, then the PA last-gates. Run [../../../../../reviews/last-gate-checklist.md](../../../../../reviews/last-gate-checklist.md) before anything leaves anyone's hands |

---

**Not run, not started, not staffed.** This file was written; the workflow was not executed, no excerpt was supplied or written, no seat was activated, nothing was installed, and no last-gated leftover-seat plan was restamped. Named gaps stay named.

Source: [../RECIPE_TEMPLATE.md](../RECIPE_TEMPLATE.md); the five contracts under [../../schemas/](../../schemas/); [../../../book-conceptual-editor.md](../../../book-conceptual-editor.md), [../../../../seats/book-conceptual-editor.md](../../../../seats/book-conceptual-editor.md), [../../../README.md](../../../README.md), [../../../../locks.md](../../../../locks.md), [../../../../leftover-write.md](../../../../leftover-write.md), [../../../../../SOURCES.md](../../../../../SOURCES.md), [../../../../../reviews/last-gate-checklist.md](../../../../../reviews/last-gate-checklist.md); the Phase 0 report for this program, carried on [PR 142](https://github.com/platformology/company-os/pull/142) and not merged.
