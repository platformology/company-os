# SOURCES.md

We searched public GitHub before writing anything in this repo, adapted the shape of what fit, and named every real gap instead of guessing. This page is the full record: what we reused, and what's still missing. Nothing here is an invented C-suite, price, client, or KPI — those are all sourced facts from Michael, or a gap named below.

## What we reused

| From | What we took | Used in |
|---|---|---|
| [dswh/company-os](https://github.com/dswh/company-os) (public fork: [kamleshvyasindia/company-os](https://github.com/kamleshvyasindia/company-os)) | `brain/company.md`, `brain/people/_template.md`, `brain/customers/_template.md`, `brain/offers.md` — one-page-per-entity pattern, "never quote a price not written here," "honest gaps beat confident blanks" | `handbook/company-facts.md`, `people.md`, `clients.md`, `offers.md` |
| [dswh/company-os](https://github.com/dswh/company-os) | `rules.md` — never / ask-first permission tiering | `handbook/locks.md` |
| [dswh/company-os](https://github.com/dswh/company-os) | `departments/_canvas-template.md`, `departments/README.md` — sensor → policy → tools → gate → learning loop shape | `handbook/weekday-loop.md`, `handbook/how-money-moves.md` |
| [dswh/company-os](https://github.com/dswh/company-os) | `reviews/README.md`, `reviews/comms-checklist.md` — the quality-gate folder pattern | `reviews/README.md`, `reviews/last-gate-checklist.md` |
| [dswh/company-os](https://github.com/dswh/company-os) | `README.md` — what's-inside table, "who this is for" framing | root `README.md` |
| [Workflowsio/company-os-starter-kit](https://github.com/Workflowsio/company-os-starter-kit) | `blueprint/INDEX.md` — content-catalog table | `handbook/README.md`, `skills/README.md` |
| [andreaswasita/copilot-cowork-dojo](https://github.com/andreaswasita/copilot-cowork-dojo) | `skills/shipping-the-deliverable/SKILL.md` — "the last gate before it ships" | `reviews/last-gate-checklist.md`, `skills/last-gate-then-stop/SKILL.md` |
| [ItamarZand88/awesome-agent-conventions](https://github.com/ItamarZand88/awesome-agent-conventions/tree/main/conventions/skill-md) | the open Agent Skills `SKILL.md` frontmatter + attribution convention | every file in `skills/` |
| [llodev/skills](https://github.com/llodev/skills) | `docs/publishing-guide.md` — attribution-first packaging | `skills/reuse-what-github-has/SKILL.md` |
| [river-labs-inc/agents](https://github.com/river-labs-inc/agents) | `customer-support-agent/system-prompt.md` — FAQ-as-gate, draft-never-send model | `skills/author-support-reply/SKILL.md` |
| [0xranx/golembot](https://github.com/0xranx/golembot) | `templates/customer-support/skills/faq-support/SKILL.md` — log what the FAQ doesn't cover | `skills/author-support-reply/SKILL.md` |
| [holacracyone/Holacracy-Constitution](https://github.com/holacracyone/Holacracy-Constitution) | `Holacracy-Constitution.md` — Role = Purpose + Domains + Accountabilities | every page in `handbook/seats/` |
| [JGalego/TeamAPI](https://github.com/JGalego/TeamAPI) | `docs/spec/teamapi-extended-v1.md` — a seat is independent of, and can be vacant of, its holder | every page in `handbook/seats/` |
| [geraldmaron/construct](https://github.com/geraldmaron/construct) | `docs/org-map.md` — the `money-flow` concept: name the obligation at the point money moves | `handbook/how-money-moves.md`, `skills/run-money-moves/SKILL.md` |
| [quivly/skills](https://github.com/quivly/skills) | `customer-engineering/meeting-prep/SKILL.md` — the pre-call brief shape, "flag gaps rather than guessing" | `skills/support-call-prep/SKILL.md` |
| [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) | `partner-built/common-room/skills/call-prep/SKILL.md` — "never invent deal context" | `skills/support-call-prep/SKILL.md` |
| [neurawork-git/n8n-autopilot](https://github.com/neurawork-git/n8n-autopilot) | `skills/stack-intake/SKILL.md` — "never invent requirements... mark genuine gaps" | `skills/blank-guest-intake/SKILL.md` |
| [lavidrori0702/tableau-dashboard-creator-skill](https://github.com/lavidrori0702/tableau-dashboard-creator-skill) | `skills/tableau-intake/SKILL.md` — required-vs-optional field table | `skills/blank-guest-intake/SKILL.md` |
| [slgoodrich/agents](https://github.com/slgoodrich/agents) | `plugins/ai-pm-copilot/skills/competitive-analysis-templates/SKILL.md` — "never fabricate, note when data is unavailable" | `skills/competitive-writing-guide/SKILL.md` |
| [seb1n/awesome-ai-agent-skills](https://github.com/seb1n/awesome-ai-agent-skills), [sales-skills/sales](https://github.com/sales-skills/sales) | `sales/lead-scoring/SKILL.md`, `skills/sales-lead-score/SKILL.md` — the fit/engagement scoring shape, inverted into a refusal since Platformology has no model | `skills/campaign-lead-scoring/SKILL.md` |
| [narrative-io/narrative-skills-marketplace](https://github.com/narrative-io/narrative-skills-marketplace) | `docs/authoring-skills.md` — "never duplicate" a reference in the skill body; point at it instead | `skills/run-uncovery`, `run-piab`, `run-campaign`, `run-retreat`, `run-money-moves`, `pa-handoff`, `run-do-this` |
| [dzhng/skills](https://github.com/dzhng/skills) | `skills/authoring/write-skills/SKILL.md` — "keep a single source of truth" | same six `run-*` / `pa-handoff` pointer skills |

Also read for structure ideas, but not directly cited to a file: [rojenwai/CompanyOS](https://github.com/rojenwai/CompanyOS).

## Named missing

Say "not recorded" or "named missing" for every item below — never fill one in from memory or a guess. Once a gap is resolved, update the file it belongs to and delete the line here.

- **Who fills each seat** in `handbook/seats/` — every seat is "not recorded" except COO (Anthony C. Garcia, public title). Jhana and Bob are not assigned to any seat.
- **Jhana's Role, Bob's Role** — not recorded (see `handbook/people.md`).
- **Live Uncovery script** — not written down.
- **Membership price** — not published.
- **PIAB cycle time, Current** — not written down.
- **Lead magnet** — has no Offers row.
- **Production stack** — not written down (Head of Engineering, Developer, CTO).
- **Studio address** — not written down.
- **June and July 2026 close status** — not closed, nothing further recorded (Controller).
- **Any savings total tied to Bench** — not sourced; no Bench connector exists (Bookkeeper).
- **A retreat date, guest list, or venue** for any specific Book Retreat — not sourced (Retreat Producer).
- **Dietary, rooming, arrival, AV, and incident fields** on the blank guest intake draft — open the Notion page directly, don't guess.
- **Five fields on the campaign lead scoring draft** — not named beyond "five," since naming them would invent structure the Notion page owns. There is no scoring model in the corpus; no criteria, weights, or thresholds exist to invent.
- **Sourced extracts for the Competitive Writing Guide's Competitive column** — filled only where Michael has provided one; blank otherwise.
- **Who the next PA is, and the current PA's tenure end date** — not sourced.
- **Any invoice, accounts-receivable figure, or savings total** tied to money moving through Platformology — not sourced.
- **Which CSO/CCO title expansion, or which VP owns what** — resolved in the handbook (`handbook/seats/cso.md`, `cco.md`, `cmo.md`, `campaign-coordinator.md`, `vp-campaigns.md`, `vp-retreats.md`); nothing left open here.
- **Two Zoom URLs for the Cornelia Choe meeting** (Thu 20 Aug 2026, 11:00–11:30am America/Denver) — unresolved; neither is picked.
- **Platinum Major List price** — no public price.
- **Track record** — uncollapsed: 124 (Dec 2022), 128 (Book Retreat), later 130–131. No single number is asserted as current.
- **KPI "Current"** — stays empty; 0 Current clients per the 18 Aug 2026 extract, not a placeholder for a future guess.
- **Hoffman's client status** — an open question, not a fact.
