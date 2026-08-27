# RECIPE_TEMPLATE

**The shape a workflow recipe takes. Headings only.** Copy this file, keep every heading, and fill each one from a source you can point at. **Candidate-visible.** Writer: docs leftover. **COO is first QC. PA last-gates.**

**This template carries no company fact.** No holder, no client, no author, no manuscript, no price, no pipeline, no KPI figure, no legal, accounting, or HR rule, and no seat's own content. Every heading below is a hole for the recipe writer to fill from a source; the prompt text under each heading says what belongs there and nothing more. If you can fill a heading from this file alone, this file is wrong.

**No SOP body lives here.** A recipe's method comes from the knowledge base its `required sources` section names. A template that supplied one would be handing every seat the same invented method.

---

## workflow_id

*The one named workflow this recipe runs, lowercase, matching the `workflow_id` pattern in [../schemas/TASK_PACKET.schema.json](../schemas/TASK_PACKET.schema.json). One recipe, one workflow_id, and it is the recipe's filename. There is no unnamed default.*

## role_slug

*The single seat slug this recipe belongs to, from the 46 in the schemas. State the seat's recorded roster status beside it — assigned, leftover-only with no live job, parked, or unassigned — and state who fills it only if that is recorded. A recipe existing for a seat does not fill, unpark, or staff it.*

## outcome

*One sentence: the single thing a completed run returns. Scope limits go here — how many items, how many passes, and what this workflow is not. If the outcome sentence needs an "and", it is two workflows.*

## required sources

*One row per source the run must read, each with its identifier and its recorded state. A source that does not exist is listed as missing, not omitted and not substituted. If a required source is missing, say what that does to the run in `stop conditions` below.*

## inputs

*The `TASK_PACKET` this recipe accepts, field by field, against [../schemas/TASK_PACKET.schema.json](../schemas/TASK_PACKET.schema.json). Name the required fields, the roster and lock values the packet must carry, and any prohibition tokens this workflow adds beyond the four baseline ones. Name what the run may not read as an input.*

## outputs (RESULT_PACKET)

*The one `RESULT_PACKET` a run returns, against [../schemas/RESULT_PACKET.schema.json](../schemas/RESULT_PACKET.schema.json). Name each field the run fills, each deliverable the packet declares, and which `outcome` values are reachable from this workflow. "Not sourced" is a first-class valid result: a packet whose every sourced field reads `"not sourced"` is well-formed and is not a failure. There is no PASS.*

*If the run can stop with a refusal, a break, or a block, name the `FAILURE_RECORD` it writes instead, against [../schemas/FAILURE_RECORD.schema.json](../schemas/FAILURE_RECORD.schema.json) — its `kind`, its `failure_class`, and its `next_owner`. If the run hands anything on, name the `HANDOFF_PACKET` against [../schemas/HANDOFF_PACKET.schema.json](../schemas/HANDOFF_PACKET.schema.json), including the receiver; if the receiver is not recorded, say so and do not name one.*

## procedure outline

*The numbered steps of the run, each one an action a reviewer could watch someone take, with the state each step leaves the run in under [../schemas/TASK_STATE.schema.json](../schemas/TASK_STATE.schema.json). Every step that can stop the run says so at the step. Outline only — the method inside a step comes from the sources named above, not from the recipe writer.*

## public acceptance criteria

*One row per criterion, each with what a reviewer opens or re-runs to settle it. Taste is not a check, and a criterion nobody can check is not a criterion. Candidate-visible: these are the criteria the seat is allowed to see. No evaluator-only material, fixture, trap, or path to one appears in a recipe.*

## missing company decisions

*Every decision this recipe needs that is not recorded, each carried by its identifier with what it blocks. Carry them; do not answer them. A recipe does not become runnable by deciding its own open questions.*

## stop conditions

*The conditions under which the run stops instead of proceeding, each paired with what the run emits when it stops — a `RESULT_PACKET`, a `FAILURE_RECORD`, or both. Absence of an input is a stop, never an invitation to supply one. A recipe with no stop condition has no floor.*

## locks

*The locks this run carries, stated as values on the packet rather than as intentions: send authority, KPI Current, activation, live-job status, recorded holder, and the definition gate where it applies. State any prohibition this recipe adds on top. The locks in the schemas are the floor, not the ceiling.*

---

**Source line.** *Every recipe ends by naming the pages and schema files it was written from, so the next reader can check it rather than believe it.*
