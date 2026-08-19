# company-os

Docs-only source of truth for how Platformology LLC runs its Grok Bot Company OS. This repo is markdown, not code — no scripts, no services, no infrastructure. If you came here looking for program code, you're in the wrong repo; see [Locks](handbook/locks.md).

## What this is

Platformology LLC operates two DBAs, **Promote a Book** and **Book Retreat** — not two companies, and not SmarterVoice. This repo is the plain-English handbook a person (or an agent acting on a person's behalf) reads before doing any work for Platformology: who the humans are, who the clients are, what the offers cost, what is locked, and which Notion page holds the real working SOP.

The living operational detail — Sales Menu line items, client records, SOP steps, meeting notes — lives in Notion, not here. This repo doesn't duplicate that. It tells you which Notion page to open for which job, and it holds the facts stable enough to check into git: legal structure, named people, the public price ladder, and the rules nobody gets to skip.

## Who this is for

- **The next PA** — read [handbook/README.md](handbook/README.md) start to finish before touching a client message or a Sales Menu number.
- **A new hire** — this is your day-one packet. If you can't answer "who are we, who can I talk to, what does this cost, what am I never allowed to do" after reading `handbook/`, the packet failed — see [reviews/last-gate-checklist.md](reviews/last-gate-checklist.md).
- **A buyer or diligence reader** — this repo, plus the [Buyer data room](https://app.notion.com/p/3c025e30d68b8135bdcdc9010e649855) Notion page, is the legible surface of the business. Nothing here is dressed up; named gaps stay named in [SOURCES.md](SOURCES.md).

## How to run it

There is nothing to install or execute. "Running" this repo means reading it in order:

1. Clone the repo.
2. Read [handbook/README.md](handbook/README.md) — it maps every other file.
3. Read [handbook/locks.md](handbook/locks.md) before you draft, send, or repo anything.
4. For a specific job, open [skills/README.md](skills/README.md) and run the matching `SKILL.md` — quoting a price, drafting a client reply, running the last gate, or writing a new doc. To find which seat owns that job, check [handbook/seats/README.md](handbook/seats/README.md) first.
5. Before anything goes to a client or gets sent externally, run it through [reviews/last-gate-checklist.md](reviews/last-gate-checklist.md).
6. Follow the Notion links inline — those pages are the live SOP; this repo does not re-host them.

## What we reused

We searched public GitHub before writing any of this. Full attribution — every repo and file adapted, plus every hole we found and left named — is in [SOURCES.md](SOURCES.md). Short version:

| Reused from | What we took the shape of |
|---|---|
| [dswh/company-os](https://github.com/dswh/company-os) (public fork: [kamleshvyasindia/company-os](https://github.com/kamleshvyasindia/company-os)) | `brain/` one-page-per-entity pattern → `handbook/company-facts.md`, `people.md`, `clients.md`, `offers.md`; `rules.md` → `handbook/locks.md`; `departments/_canvas-template.md` loop shape → `handbook/weekday-loop.md`; `reviews/` gate pattern → `reviews/` |
| [holacracyone/Holacracy-Constitution](https://github.com/holacracyone/Holacracy-Constitution) | the Role = Purpose + Domains + Accountabilities shape → every page in `handbook/seats/` |
| [JGalego/TeamAPI](https://github.com/JGalego/TeamAPI), `docs/spec/teamapi-extended-v1.md` | the seat-is-independent-of-its-holder model (a seat can be vacant) → `handbook/seats/` |
| [Workflowsio/company-os-starter-kit](https://github.com/Workflowsio/company-os-starter-kit) | `blueprint/INDEX.md` content-catalog table → `handbook/README.md` |
| [andreaswasita/copilot-cowork-dojo](https://github.com/andreaswasita/copilot-cowork-dojo), `skills/shipping-the-deliverable/SKILL.md` | the "last gate before it ships" checklist shape → `reviews/last-gate-checklist.md`, `skills/last-gate-then-stop/SKILL.md` |
| [river-labs-inc/agents](https://github.com/river-labs-inc/agents), `customer-support-agent/system-prompt.md` | the FAQ-as-gate, draft-never-send model → `skills/author-support-reply/SKILL.md` |
| [0xranx/golembot](https://github.com/0xranx/golembot), `templates/customer-support/skills/faq-support/SKILL.md` | log-what's-not-covered pattern → `skills/author-support-reply/SKILL.md` |
| [ItamarZand88/awesome-agent-conventions](https://github.com/ItamarZand88/awesome-agent-conventions/tree/main/conventions/skill-md), [llodev/skills](https://github.com/llodev/skills) `docs/publishing-guide.md` | the `SKILL.md` frontmatter + attribution convention → every file in `skills/` |

We did not copy anyone's invented C-suite, prices, clients, or KPIs. Every fact in `handbook/` is a fact Michael gave us, or a gap we're naming as missing. Full attribution for every file: [SOURCES.md](SOURCES.md).

## Existing Company OS (Notion — the source of truth)

This repo is the git-native front door. The working pages already exist in Notion and are not rewritten here:

- [Company OS home](https://app.notion.com/p/3c025e30d68b81cdbad7fdf5912e3ca3)
- [Sales Menu](https://app.notion.com/p/3c025e30d68b817dae2eeb55c5902ad7)
- [Do this](https://app.notion.com/p/3c025e30d68b8142a971ccdb0d657b22)
- [If a client writes](https://app.notion.com/p/3c025e30d68b81ada7b7cbf1d50b0d9f)
- [Campaign SOP](https://app.notion.com/p/3c025e30d68b81ea99c0dcf96db7cd2e)
- [Retreat SOP](https://app.notion.com/p/3c025e30d68b8185b9a9f19dd56389e5)
- [Uncovery SOP](https://app.notion.com/p/3c125e30d68b815d9dbbd7e59102af3e)
- [PIAB SOP](https://app.notion.com/p/3c125e30d68b81d5beecda81a111e6b3)
- [How money moves](https://app.notion.com/p/3c125e30d68b81b49524fe7bc9f65c81)
- [Grok Bot staff](https://app.notion.com/p/3c125e30d68b81dc9116e2e62b47f143)
- [PA handoff](https://app.notion.com/p/3c125e30d68b8138a686fd8a52313333)
- [Buyer data room](https://app.notion.com/p/3c025e30d68b8135bdcdc9010e649855)

## Locks (read before you do anything)

No send without Michael. No program GitHub. No VMs. No GKE. M5 stays parked until the machine is in hand. Blue Sky stays off the LLC books. Full list: [handbook/locks.md](handbook/locks.md).
