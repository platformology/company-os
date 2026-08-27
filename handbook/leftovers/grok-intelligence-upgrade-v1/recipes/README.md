# recipes/ — the Phase 1 recipe set

Two files: the shape a workflow recipe takes, and the one pilot workflow recipe written into that shape. **That is the whole Phase 1 recipe set**, and it is the set the Phase 0 report proposed — not a first instalment of a larger one.

Company: **Platformology LLC**. **Promote a Book** and **Book Retreat** are DBAs.

## The two files

| File | What it is | Visibility | Writer | Reviewer |
|---|---|---|---|---|
| [RECIPE_TEMPLATE.md](RECIPE_TEMPLATE.md) | The shape a workflow recipe takes — headings only, with a prompt under each saying what belongs there. **It carries no company fact and no SOP body** | Candidate-visible | Docs leftover | COO first QC, then PA last-gate |
| [book-conceptual-editor/bce-structural-read-excerpt-v1.md](book-conceptual-editor/bce-structural-read-excerpt-v1.md) | The one pilot workflow recipe: a single-excerpt structural read of owner-supplied evaluation material, returning one `RESULT_PACKET`. **Written, not run** | Candidate-visible | Docs leftover | COO first QC, then PA last-gate |

## What is deliberately not here

- **Not 3–5 recipes per seat.** The owner's brief for this unit places that in Phase 3. Writing them now would be doing later work early, and would make this set look incomplete when it is not.
- **No recipe for the two parked seats**, `head-of-engineering` and `developer`. They stay parked, and a recipe is a thing to run.
- **No recipe for the three leftover-only seats with no live job**, `head-of-demand`, `head-of-sales`, and `sdr`. There is no live job to write one against.
- **No recipe for the three definition-gated seats**, `cso`, `cco`, and `pendulum-wiki`. What each means is not recorded, and a recipe would have to invent it.
- **No routing, knowledge, examples, corrections, metrics, handoffs, or reports directory**, and nothing added to [../schemas/](../schemas/).
- **No evaluator-only material** — not a fixture, not a trap, and not a path to one. Both files above are candidate-visible in full, which is what lets this folder be handed over whole.

## The contracts these recipes are written against

Both files cite the five packet schemas by path rather than restating them. Those contracts were **last-gated on [PR 143](https://github.com/platformology/company-os/pull/143)** under [../schemas/](../schemas/), and **this work reuses them unchanged** — no schema is rewritten, extended, or re-specified here.

| Contract | Used for |
|---|---|
| [../schemas/TASK_PACKET.schema.json](../schemas/TASK_PACKET.schema.json) | The input a recipe accepts, and the locks it carries |
| [../schemas/TASK_STATE.schema.json](../schemas/TASK_STATE.schema.json) | The state each procedure step leaves the run in |
| [../schemas/RESULT_PACKET.schema.json](../schemas/RESULT_PACKET.schema.json) | The one output a run returns, where "not sourced" is a valid result |
| [../schemas/HANDOFF_PACKET.schema.json](../schemas/HANDOFF_PACKET.schema.json) | The handoff — and, in the pilot, the reason none is emitted |
| [../schemas/FAILURE_RECORD.schema.json](../schemas/FAILURE_RECORD.schema.json) | What a refusal, a block, or a break records |

**Because PR 143 is not merged**, this pull request is stacked on that branch so every schema path above is openable here. Neither PR is merged by this work.

## What this folder does not do

It runs nothing. The pilot recipe was **written and not executed**: no excerpt was supplied or written, no `RESULT_PACKET` was produced, and no acceptance run happened. Zero runs is the honest state, and **zero runs is not a pass**.

It activates nobody, staffs no seat, unparks no seat, and creates no live job. It installs nothing and adds no dependency. It invents no company fact — no holder, client, author, manuscript, price, pipeline, KPI figure, or legal, accounting, or HR rule — and **KPI Current stays empty**, which is not 0. No last-gated leftover-seat plan is restamped, and the original workforce pack is untouched.

**COO is first QC. PA last-gates.** Run [../../../../reviews/last-gate-checklist.md](../../../../reviews/last-gate-checklist.md) before anything leaves anyone's hands. **Nothing sends.**

Named gaps stay named. Full list: [../../../../SOURCES.md](../../../../SOURCES.md).
