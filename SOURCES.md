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

Searched and deliberately **not** adapted, so they get no row above: [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills), [kostja94/marketing-skills](https://github.com/kostja94/marketing-skills), and [guilhermemarketing/esc-skills](https://github.com/guilhermemarketing/esc-skills). All three generate ICPs, personas, ad creative, and landing-page copy from templates; the CMO seat needs the opposite of that, so nothing was taken. `skills/run-cmo/SKILL.md` names them for the same reason this note does — so the next person doesn't re-run the same search.

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
- The Competitive Writing Guide's Competitive column, filled only from a sourced extract.
- June and July 2026 are not closed.
- No Bench savings total, and no Bench connector.
- Who the next PA is, and the current PA's tenure end date.
- No invented invoice, accounts-receivable figure, or savings total.
- Blue Sky stays off the LLC books.
- Three of 23 seats have no dedicated seat router yet — Head of Content (`run-content`), CHRO (`run-chro`), People Ops (`run-people-ops`). The other 20 seats each have one. See [handbook/seat-job-map.md](handbook/seat-job-map.md) for the seat-side view and [skills/README.md](skills/README.md) for the skill-side view; both name these three as missing rather than pointing at a page that doesn't exist.
