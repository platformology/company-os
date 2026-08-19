# Sources

We searched public GitHub before writing these pages. Facts inside are Michael's, or named missing. Nobody else's C-suite, prices, clients, or KPIs were copied.

This page holds one table and one list, and nothing else: every shape we reused, then every gap we left named. If a skill on this tree cites a repo, that repo has a row in the table. If a fact is missing, it is named once in the list rather than filled in from a guess.

## Reused shapes

| Repo | What we took |
|---|---|
| [dswh/company-os](https://github.com/dswh/company-os) (fork: [kamleshvyasindia/company-os](https://github.com/kamleshvyasindia/company-os)) | The one-page-per-entity `brain/` pattern, "never quote a price not written here," the `rules.md` never/ask-first tiering, the sensor→policy→tools→gate→learning loop shape, the `reviews/` quality-gate pattern, and the README framing |
| [Workflowsio/company-os-starter-kit](https://github.com/Workflowsio/company-os-starter-kit) | The `blueprint/INDEX.md` content-catalog table |
| [holacracyone/Holacracy-Constitution](https://github.com/holacracyone/Holacracy-Constitution) | Role = Purpose + Domains + Accountabilities |
| [JGalego/TeamAPI](https://github.com/JGalego/TeamAPI) | A seat is independent of, and can be vacant of, its holder |
| [andreaswasita/copilot-cowork-dojo](https://github.com/andreaswasita/copilot-cowork-dojo) | "The last gate before it ships" checklist shape |
| [ItamarZand88/awesome-agent-conventions](https://github.com/ItamarZand88/awesome-agent-conventions/tree/main/conventions/skill-md) | The `SKILL.md` frontmatter + attribution convention |
| [llodev/skills](https://github.com/llodev/skills) | Attribution-first packaging |
| [river-labs-inc/agents](https://github.com/river-labs-inc/agents) | The FAQ-as-gate, draft-never-send model |
| [0xranx/golembot](https://github.com/0xranx/golembot) | Logging what the FAQ doesn't cover |
| [geraldmaron/construct](https://github.com/geraldmaron/construct) | The `money-flow` concept: name the obligation at the point money moves |
| [quivly/skills](https://github.com/quivly/skills) | The pre-call brief shape; "flag gaps rather than guessing" |
| [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) | "Never invent deal context" |
| [neurawork-git/n8n-autopilot](https://github.com/neurawork-git/n8n-autopilot) | "Never invent requirements... mark genuine gaps" |
| [lavidrori0702/tableau-dashboard-creator-skill](https://github.com/lavidrori0702/tableau-dashboard-creator-skill) | The required-vs-optional field table |
| [slgoodrich/agents](https://github.com/slgoodrich/agents) | "Never fabricate; note when data is unavailable" |
| [seb1n/awesome-ai-agent-skills](https://github.com/seb1n/awesome-ai-agent-skills) | The fit/engagement scoring shape, inverted into a refusal |
| [sales-skills/sales](https://github.com/sales-skills/sales) | The same scoring shape, inverted into a refusal |
| [narrative-io/narrative-skills-marketplace](https://github.com/narrative-io/narrative-skills-marketplace) | "Never duplicate" a reference in the skill body |
| [dzhng/skills](https://github.com/dzhng/skills) | "Keep a single source of truth" |
| [rojenwai/CompanyOS](https://github.com/rojenwai/CompanyOS) | Read for structure ideas; not cited to a specific file |
| [0xdarkmatter/claude-mods](https://github.com/0xdarkmatter/claude-mods) | The token-cheap loop discipline: "the cheapest lever is cadence... put the cheap model on the maker" → `handbook/cheap-loop.md` |
| [Oruga420/claude-code-skills](https://github.com/Oruga420/claude-code-skills) | The zero-work-run question and the one-agent, no-fan-out rule — both inverted or reused straight → `handbook/cheap-loop.md`, `skills/run-always-on/SKILL.md` |
| [tonone-ai/tonone](https://github.com/tonone-ai/tonone) | The meeting-definition table shape, inverted from "design the cadence" into "point at the cadence Michael already locked" → `skills/run-meetings/SKILL.md` |
| [athola/claude-night-market](https://github.com/athola/claude-night-market), `plugins/abstract/skills/skill-authoring/modules/advanced-patterns.md` | The Activation Gate shape — if the condition fails, stop and say the skill doesn't apply rather than quietly proceeding on a smaller version of the ask → `skills/run-engineering/SKILL.md`, `skills/run-developer/SKILL.md` |
| [blouargant/yoke](https://github.com/blouargant/yoke), `docs/skills.md` | The "Hard rules" list plus a closing one-line verdict → `skills/run-engineering/SKILL.md` |
| [designgrappler/agent-skills](https://github.com/designgrappler/agent-skills), `skills/add-specialist/SKILL.md` | The Scope Lock shape: work only on what's declared, and flag anything outside it instead of making the change → `skills/run-developer/SKILL.md` |
| [judicialmind/legal-skills](https://github.com/judicialmind/legal-skills), `skills/due-diligence/SKILL.md` | Data-room organization: a diligence response is a checklist of what exists, not a narrative you write → `skills/run-buyer-packet/SKILL.md` |
| [latour-ai/skills](https://github.com/latour-ai/skills), `hedge-fund-diligence/SKILL.md` | Separating what is claimed, what the evidence supports, and what still needs diligence — the gap becomes an ask-next list, never an estimate → `skills/run-buyer-packet/SKILL.md` |
| [jwbreunsbach/uncommon-cco-library](https://github.com/jwbreunsbach/uncommon-cco-library), `skills/cs-launch-enablement.md` | The own-it / escalate-it split written as unambiguous rules, and "flag for review" in place of a guess → `skills/run-cco/SKILL.md`, `skills/run-author-success/SKILL.md`, `skills/run-client-success/SKILL.md` |
| [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills), `c-level-advisor/skills/chief-customer-officer-advisor/SKILL.md` and `business-growth/skills/customer-success-manager/SKILL.md` | The shape of a customer seat — a short list of standing decisions, and one seat watching how engagements are going. Their health scores, churn tiers, and expansion metrics were left behind and inverted into a refusal, the same way `campaign-lead-scoring` inverts lead scoring → `skills/run-cco/SKILL.md`, `skills/run-author-success/SKILL.md`, `skills/run-client-success/SKILL.md` |
| [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills), `business-operations/skills/capacity-planner/SKILL.md`, `business-operations/skills/vendor-management/SKILL.md`, and `business-operations/skills/knowledge-ops/SKILL.md` | "If you only have averages, stop and pull the distribution — single-point demand estimates are the most expensive anti-pattern in ops," which is why the CHRO seat refuses to size a three-person roster; vendor records come from the vendor's own source, "not invented"; and the librarian framing that the job is the artifacts operators consume, findable and with a named owner → `skills/run-chro/SKILL.md`, `skills/run-people-ops/SKILL.md`, `skills/run-content/SKILL.md` |
| [microsoft/github-copilot-modernization](https://github.com/microsoft/github-copilot-modernization), `plugins/github-copilot-modernization/skills/team-charters/SKILL.md` | A charter is Mission plus what the role owns plus a Core Principle naming what the role must **not** do — "ownership boundaries are strict" → `skills/run-chro/SKILL.md` |
| [mohitagw15856/pm-claude-skills](https://github.com/mohitagw15856/pm-claude-skills), `skills/role-redesign-for-ai/SKILL.md` | "Do not write 'focus on higher-value work' without naming the work" → `skills/run-chro/SKILL.md` |
| [onvoyage-ai/gtm-engineer-skills](https://github.com/onvoyage-ai/gtm-engineer-skills), `audit-content/SKILL.md` | "Don't rewrite the article — your job is to audit and report, not to edit," which is the librarian-not-writer line the content seat holds → `skills/run-content/SKILL.md` |
| [alelaguard/agentguards-plugins](https://github.com/alelaguard/agentguards-plugins), `claude/skills/guardrails/SKILL.md` | Run the check *before* the action rather than after, and answer in one fixed shape when it blocks — kept, but rewritten as a sentence a person says out loud instead of a tool call → `skills/check-locks/SKILL.md` |
| [arthursilas-ai/agent-preflight](https://github.com/arthursilas-ai/agent-preflight), `README.md` | The blocked verdict that names what to resolve, and "every finding carries a fix, not just a complaint" — so a refusal names where the ask goes next → `skills/check-locks/SKILL.md` |
| [qa-aman/claude-skills](https://github.com/qa-aman/claude-skills), `skills/by-role/marketing/customer-persona/SKILL.md` | One file owns the field list and its order, and everything else is "Read only. Never edit, reorder, or delete"; a slot with no real quote behind it is marked as needing input instead of filled "from the desk," because a later writer reads invented language as observed speech and puts it into public copy. Its rival-alternatives step was left behind → `skills/competitive-writing-guide/SKILL.md` |
| [Unabyss/unabyss-skills](https://github.com/Unabyss/unabyss-skills), `brand-voice/SKILL.md` | A fixed field list describing how one reader wants to be written to, where "every observation grounded in an actual sample — no invented characterizations," and thin sourcing is named as thin rather than filled in → `skills/competitive-writing-guide/SKILL.md` |
| [nicholasswhite/agent-readiness-checklist](https://github.com/nicholasswhite/agent-readiness-checklist), `CHECKLIST.md` | Grouped checks that only pass on something you can observe — "results leave reviewable diffs, command output, logs, or artifacts," "facts, inferences, and unknowns are distinguished," and the closing note that an unchecked item is a prompt to investigate rather than proof of a defect → `handbook/runtime.md` |
| [DenisSergeevitch/agents-best-practices](https://github.com/DenisSergeevitch/agents-best-practices), `references/mvp-agent-blueprint.md` | The "Minimal implementation path — recommended build order," where the working baseline is built first and tracing, planning, connectors, and evals come after. That ordering is why `handbook/runtime.md` builds brain, hands, wiring, and guts before any business, marketing, or R&D plan gets written. Its harness internals — loops, tool registries, permission engines, budgets — were left behind; this repo is docs only and installs nothing → `handbook/runtime.md` |
| [petekp/agent-skills](https://github.com/petekp/agent-skills), `skills/autonomous-agent-readiness/SKILL.md` | The per-dimension "Current state: what exists today / Gap: what's missing" pair, used under each of the four runtime pieces. Its 0–3 dimension scores and overall X/36 readiness score were left behind — a done-check on `handbook/runtime.md` is observable or it is nothing, and no number goes in one → `handbook/runtime.md` |
| [Moonweave-AI/governance](https://github.com/Moonweave-AI/governance), `05-Knowledge/en/01-Documentation-Guide.md` | "Documentation has status and validity period... documentation without status cannot be trusted," plus "use relative links to reference documents within the same repository" — so the four sister pages on `handbook/runtime.md` are linked relatively and each one says where it actually is: on `main`, or last-gated and in QC on its own PR. Its Draft / Active / Deprecated / Superseded / Archived vocabulary was left behind for the two states this repo really has → `handbook/runtime.md` |

Searched and deliberately **not** adapted, so they get no row above: [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills), [kostja94/marketing-skills](https://github.com/kostja94/marketing-skills), and [guilhermemarketing/esc-skills](https://github.com/guilhermemarketing/esc-skills). All three generate ICPs, personas, ad creative, and landing-page copy from templates; the CMO seat needs the opposite of that, so nothing was taken. `skills/run-cmo/SKILL.md` names them for the same reason this note does — so the next person doesn't re-run the same search.

`skills/competitive-writing-guide/SKILL.md` no longer cites [slgoodrich/agents](https://github.com/slgoodrich/agents), `plugins/ai-pm-copilot/skills/competitive-analysis-templates/SKILL.md`. A competitive-analysis kit is the wrong shape for that job: the guide is about one buying style, not a rival company, and the kit's shape pulls a reader toward a teardown. Searched and not adapted there. The row above stays because `skills/run-clients/SKILL.md` and `skills/run-demand/SKILL.md` still use its never-fabricate line.

## Named missing

- Live Uncovery script.
- Membership price.
- PIAB cycle time.
- Lead magnet has no Offers row.
- Jhana's Role.
- Bob's Role.
- Production stack.
- Studio address.
- Two unresolved Zoom URLs for Cornelia Choe's Thu 20 Aug 2026, 11:00–11:30am America/Denver meeting — neither is picked.
- Platinum Major List has no public price.
- Track record is uncollapsed: 124 (Dec 2022), 128 (Book Retreat), later 130–131 — no single number is current.
- KPI "Current" stays empty.
- Hoffman's client status is a question, not a fact.
- Who fills each seat, except COO (Anthony C. Garcia).
- Head of Demand, Head of Sales, and SDR are unassigned — no volume, pipeline, or score invented for them.
- A retreat date, guest list, or venue for any specific Book Retreat.
- The guest intake draft's dietary, rooming, arrival, AV, and incident fields.
- Five unnamed fields on the campaign lead scoring draft, and no scoring model in the corpus.
- The Competitive Writing Guide's Competitive buying-style answers for the same fields its Methodical list names, filled only from a sourced extract.
- June and July 2026 are not closed.
- No Bench savings total, and no Bench connector.
- Who the next PA is, and the current PA's tenure end date.
- No invented invoice, accounts-receivable figure, or savings total.
- Blue Sky stays off the LLC books.
- A link to the Notion Clients database — the CRM itself — is not recorded in this repo.
- Michael's 2021–2026 files, without which there is no current-client history to give.
- The named leftovers sitting behind most seats' jobs — this repo lists the router, not the queue.
- All four runtime sister pages — `handbook/runtime-brain.md`, `handbook/runtime-body.md`, `handbook/runtime-wiring.md`, `handbook/runtime-guts.md` — are on `main`, so none of them is a gap. Nobody re-derives what they say or calls them missing. The local hand itself is not a gap either — it is a locked decision waiting on Michael's go, per `handbook/locks.md` and `handbook/runtime-brain.md`.
