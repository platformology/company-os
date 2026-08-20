# ClawHub — what actually exists, per seat

A shopping list. **Nobody is shopping.** [locks.md](../locks.md) and [runtime-openclaw.md](../runtime-openclaw.md) both say the same thing about the public registry — our skills are written here, credited in [SOURCES.md](../../SOURCES.md), and reviewed by a person — so nothing below gets installed. This page exists so the next person does not re-run the search, and so a real gap can be told apart from a gap nobody looked for.

Every slug on this page was returned by ClawHub's own public search on **20 Aug 2026**, under the owner handle shown. Where a search came back with nothing that fits, the row says **not confirmed on ClawHub — named missing**, and it stays that way. Nothing on this page was made up to fill a row.

## How to read a row

**Refs are `@owner/slug`, always.** A bare slug is not an address on ClawHub: ask the registry for `notion` and it answers that it found several and wants to know which one. Two different people own a skill called `notion`, three own one called `pdf`. Write the owner or you have written nothing.

Three verdicts, and only three:

- **Shape only** — the thing exists, the shape is right, a person could read it for ideas. Still not installed.
- **DENIED** — it sends, posts, publishes, replies, or writes to something we only read. The lock is *no send without Michael*, and a skill that sends is a lock break with a nice description.
- **Refused** — the shape is wrong for this company, or the seat is parked or unassigned. Named so nobody proposes it again.

Two standing cautions that travel with every row. ClawHub is **open by default**: their own docs say anyone can upload, publishing needs only a GitHub account old enough to pass an upload gate, and automated scans can pull a release out of the public catalog after the fact. And their own security note says to treat a third-party skill as untrusted code. We agree, and we go one further by not fetching it.

## "Prefer official / openclaw" came up empty

Worth saying plainly, because it was the first thing asked for. The OpenClaw docs use `@openclaw/demo` as an example in their quick start; a registry lookup on that exact ref returns nothing, and no `@openclaw/*` skill matched any job below. ClawHub's site has an **Official** tab, and it returned nothing this repo could read from outside a browser, so **no row below is claimed as official.** The nearest thing is a handful of company-looking accounts that do own skills — `anthropics`, `openai`, `claude-office-skills`, `googleworkspace-bot` — and none of them is OpenClaw. Three of their skills are named below on that basis and no other.

## The six boring ones, answered directly

Michael named six. Here is what is actually on the registry for each.

| The job | What exists | Verdict |
|---|---|---|
| **Calendar read** | `@porteden/calendar-skill` — "list, search, or read calendar events," Google plus Outlook and Exchange. Also `@xejrax/brainz-calendar` (Google Calendar through `gcalcli`) and `@byungkyu/google-calendar-api` (managed OAuth). | **Shape only, read verbs.** All three also create, update, or delete events. Every write verb is **DENIED** — the seats read the calendar that already exists and never make a meeting to fill a phase. |
| **Gmail draft** | `@officialdelta/gmail-secretary` — triage, labels, and draft replies, and its own description says it **never auto-sends**. | **Shape only**, and the only Gmail skill found that promises not to send. `@byungkyu/gmail` and `@hith3sh/gmail-email` both send and reply: **DENIED**. `@porteden/gmail-cli` reads and triages but also sends, replies, forwards, and deletes: **DENIED** on all four. |
| **Notion read** | `@byungkyu/notion-api-skill` — queries databases, searches pages, reads workspace content, and says write operations need explicit confirmation of the target. `@dimagious/notion-skill` — schema diffs before structural changes, append-first writes. | **Shape only.** The first is the closest thing to read-only on the registry; the second is the most careful write shape found, and it is still a write shape. `@steipete/notion` and `@hith3sh/notion-pages` create and modify: **DENIED**. |
| **FAQ** | `@imbing/bo-faq-bot` — build and query a FAQ knowledge base out of markdown files. | **Shape only.** Our FAQ is the Notion **If a client writes** page, and it is a *gate*, not a corpus to rebuild. `@mariusfit/whatsapp-faq-bot` is the same engine wired to WhatsApp: **DENIED — channel**. `@zenobiazizi/skill-faq-mining` mines a FAQ out of past support logs, and we have no log corpus to mine. |
| **Last gate** | Nothing that matches. The closest are generic task checklists: `@welliu/checklist` and `@deciqai/checklist`. | **Not confirmed on ClawHub — named missing.** A checklist that runs *and can refuse to ship* is not on the registry. Ours is [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md) and [last-gate-then-stop](../../skills/last-gate-then-stop/SKILL.md), and it stays ours. |
| **Offer ladder** | Nothing that matches. Everything called pricing *sets* prices: `@ivangdavila/pricing`, `@coreyhaines31/pricing-strategy`. | **Not confirmed on ClawHub — named missing.** Our prices are already set and are quoted off one page, both numbers where the ladder shows two. A skill that recommends a price is the opposite job. [run-offers](../../skills/run-offers/SKILL.md) and [place-on-offer-ladder](../../skills/place-on-offer-ladder/SKILL.md) stay ours. |

Two of the six come back empty. That is the honest result, and it is the useful half of this page.

## Per seat

Same twenty-three, same order as [desks/README.md](../desks/README.md).

### PA

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Read the **Do this** page | `@byungkyu/notion-api-skill` | Shape only, read side |
| Read the existing calendar slots | `@porteden/calendar-skill` | Shape only, read verbs; **DENIED** on create and update |
| Draft in Gmail, never send | `@officialdelta/gmail-secretary` | Shape only — never auto-sends |
| Block time on the calendar | `@zvirb/executive-assistant-time-blocking` | **DENIED — writes the calendar.** This seat reads the cadence off the slots that exist |
| A day list of its own | `@ivangdavila/task-list` | **Refused.** The do-this page is the list. A second list is a second source of truth |
| The handoff pack | — | **Not confirmed on ClawHub — named missing.** [pa-handoff](../../skills/pa-handoff/SKILL.md) stays ours |

### COO

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Read **Grok Bot staff**, **Company OS home** | `@byungkyu/notion-api-skill` | Shape only, read side |
| Read the meetings that already exist | `@porteden/calendar-skill` | Shape only, read verbs; **DENIED** on create — no meeting gets made to fill a phase |
| Write a pass up from meetings that happened | `@claude-office-skills/meeting-notes`, `@mohitagw15856/meeting-notes` | Shape only. Both work off notes of a meeting that already happened, which is the right direction |
| First QC on a docs change | `@anthropics/code-review` | **Refused — wrong artifact.** It reviews code. Docs QC here is the COO's own read, then the PA's gate |

### CMO

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Read the **Sales Menu** | `@byungkyu/notion-api-skill` | Shape only, read side |
| The offer ladder | `@ivangdavila/pricing`, `@coreyhaines31/pricing-strategy` | **Refused — wrong shape.** Both decide what to charge. Ours is decided; the job is quoting it correctly |
| Positioning voice | `@mupengi-bot/brand-voice`, `@leooooooow/brand-voice-guide` | **Refused — wrong shape.** Both *generate* a voice guide. Ours is the Competitive Writing Guide draft, filled only from a sourced extract, and its blanks stay blank. Same reason [SOURCES.md](../../SOURCES.md) already records three marketing kits searched and not adapted |

### Head of Content

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Read the files already in Drive | `@berkgungor/google-drive-composio` — browse folders and read the files inside them | Shape only, read side; **DENIED** on upload and share |
| Anything broader on Drive | `@hith3sh/google-drive-files` | **DENIED — manages permissions, uploads, changes sharing** |
| Catalog a library without rewriting it | `@ncreighton/content-audit-expert`, `@mohitagw15856/ai-content-audit` | Shape only, and the right instinct: audit and report, do not edit. That is the librarian-not-author rule this seat already holds |
| Read a corpus PDF | `@anthropics/pdf` | Shape only |
| A catalog of a 27-year private archive | — | **Not confirmed on ClawHub — named missing.** No public skill knows our corpus, and none is going to |

### Head of Demand — unassigned

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Anything inbound | `@luigi08001/lead-scoring` and a long list beside it | **Refused — the seat is unassigned.** There is no inbound volume, lead count, or channel recorded. That skill also scores into HubSpot, which is closed here. Installing something does not staff a seat |

### CSO

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Read Notion **Clients** for status | `@byungkyu/notion-api-skill` | Shape only, read side |
| Run a CRM | `@ivangdavila/crm` — contacts, deals, pipeline stages, forecasts | **DENIED.** The CRM is Notion Clients and no new one gets added. This seat answers "no pipeline recorded" rather than producing a forecast |
| Track a pipeline | `@1kalin/sales-pipeline-tracker` | **Refused.** No pipeline exists to track, and one does not get invented to give the tool something to do |
| Place someone on a rung | — | **Not confirmed on ClawHub — named missing.** [place-on-offer-ladder](../../skills/place-on-offer-ladder/SKILL.md) stays ours |

### Head of Sales — unassigned

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Outbound | `@coreyhaines31/cold-email` | **DENIED — sends**, twice over: the seat is unassigned and nothing goes out without Michael |
| Paid discovery | `@mohitagw15856/discovery-call-prep`, `@staybased/client-discovery` | **Refused — the seat is unassigned.** The live Uncovery script is a named gap in [SOURCES.md](../../SOURCES.md), and an unassigned seat does not close it with a generic sales framework |

### SDR — unassigned

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Score leads | `@luigi08001/lead-scoring` | **Refused.** No scoring model exists in the corpus, and [campaign-lead-scoring](../../skills/campaign-lead-scoring/SKILL.md) exists specifically to refuse building one. The seat is unassigned besides |

### CFO

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| A CFO's whole job | `@ivangdavila/cfo` — forecasts cash, computes runway and burn, runs the close, models a fundraise | **DENIED.** Every verb in that list produces a number this repo does not have. A dressed-up figure is worse than a blank, because diligence finds it |
| Read **How money moves** | `@byungkyu/notion-api-skill` | Shape only, read side |
| A Bench connector | — | **Not confirmed on ClawHub — named missing**, and it stays missing. Bench is opened by a person by hand or not at all |

### Controller

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| A month-end close checklist | `@anthropics/close-management` — sequencing, dependencies, status tracking, and its own note that it is not financial advice | Shape only, and the closest fit on this page: a checklist that carries no numbers |
| Same, firm-flavoured | `@samledger67-dotcom/financial-close-checklist` | Shape only |
| Close June and July 2026 | `@anthropics/month-end-prep` | **Refused — it needs QuickBooks and a payment processor connected**, and neither is on this Mac. June and July stay "not closed," which is the answer, not a gap |

### Bookkeeper

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Chart of accounts, categorisation | `@mohitagw15856/bookkeeping-categorization`, `@jk-0001/bookkeeping-basics` | Shape only. Both assume a ledger you can read; Bench has no connector, so there is nothing to categorise from here |
| Reconcile bank feeds and receipts | `@kyro-ma/bookkeeping-reconciliation-helper` | Shape only, same caveat |
| Invoices | `@ivangdavila/invoice` — create **and send** invoices | **DENIED — sends** |
| Log and report spending | `@ivangdavila/expenses` | **Refused.** There is no sourced spend figure here, and no savings total. "Nobody read the ledger" is a finished answer |

### CTO

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Anything installable | everything on the registry | **DENIED.** This seat's whole job is naming the lock that stops an ask. A registry install is that ask |
| Operating OpenClaw itself | `@bkf-gitty/claw-update-runbook` — updating an OpenClaw instance and debugging gateway startup after | Named for the record, and **not needed: nothing is installed.** If Michael ever says go, this is the first public thing worth reading |
| Designing a seat chart that routes work | `@delasy/agent-org-chart` — "pick roles by what they refuse, wire reporting lines, bound hand-offs, and place human gates" | Shape only, and worth naming because it is the closest public description of what [seats/](../seats/README.md) and [runtime-wiring.md](../runtime-wiring.md) already did by hand. The work is done; this would be a second opinion, not a tool |
| A runbook shape | `@anthropics/runbook` | Shape only |

### Head of Engineering — parked · Developer — parked

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Code review, deploys, stacks | `@anthropics/code-review` and hundreds beside it | **Refused — both seats are parked.** There is no recorded stack and no machine to write code on. Installing a code skill would break two locks at once: the registry install, and starting parked work |

### CCO

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Read what came in, in Gmail | `@officialdelta/gmail-secretary` | Shape only — never auto-sends |
| The FAQ as a gate | `@imbing/bo-faq-bot` | Shape only. Ours is a Notion page and it is the gate; not in the FAQ means flag it for Michael, not answer it |
| Triage and route | `@anugotta/customer-support-autopilot` — classify, draft, route escalations by risk | Shape only, and the own-it-or-escalate-it split is right. Its SLA and risk scoring are **refused** — no health score exists here and none gets invented |
| Judge how an engagement is going | `@ivangdavila/customer-support` | **Refused — wrong source.** Author success is checked against [clients.md](../clients.md), never against a folder name and never against HubSpot |

### Head of Author Success

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Read the FAQ, read Gmail | `@byungkyu/notion-api-skill`, `@officialdelta/gmail-secretary` | Shape only, read and draft sides |
| Read an existing call's time | `@porteden/calendar-skill` | Shape only, read verbs |
| Prep for a call | `@mohitagw15856/discovery-call-prep`, `@staybased/client-discovery` | **Refused — both are sales discovery.** Cornelia Choe is Alumni: support, not a pitch. [support-call-prep](../../skills/support-call-prep/SKILL.md) stays ours |

### Client Success

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Draft a reply and leave it | `@officialdelta/gmail-secretary` | Shape only — never auto-sends, which is this seat's whole constraint |
| Anything that replies or forwards | `@porteden/gmail-cli`, `@hith3sh/gmail-email` | **DENIED — send, reply, forward.** This seat does not send, post, schedule, or reply directly, and never claims a message went out |
| Write the reply well | `@tangentus/editor-in-chief`, `@ivangdavila/writing` | Shape only. See the cross-seat note below |

### CHRO · People Ops

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Read **Grok Bot staff** | `@byungkyu/notion-api-skill` | Shape only, read side |
| HR policy | `@1970168137/hr-policy-generator` | **Refused.** Three people and two vendors do not get a policy suite. Today's thin scope is an honest state, not a gap |
| Hiring | `@anthropics/recruiting-pipeline`, `@agistack/recruiting` | **Refused.** No hiring is recorded. A pipeline with nobody in it is an invented org chart with extra steps |
| Keep a roster honest | — | **Not confirmed on ClawHub — named missing.** [run-staff](../../skills/run-staff/SKILL.md) stays ours, because the job is refusing to fill Jhana's and Bob's Role, and no public skill refuses anything |

### VP Campaigns · Campaign Coordinator

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Run a campaign off a package | `@nadavnaveh/campaign-management` — read campaign packages, manage state, report | Shape only. Ours runs off the **Campaign SOP** in Notion, which this repo does not restate |
| Write the SOP down | `@balkanblbn/sop-architect`, `@anthropics/process-doc` | Shape only, and not needed: the SOP exists and VP Campaigns owns it. Neither seat rewrites it |
| A book launch | `@charlie-morrison/book-launch-coach`, `@jinhuadeng/book-launch-campaign-kit` | **Refused.** Both generate positioning, copy, and promo assets from templates. That is the shape the CMO seat already refused, and a campaign here runs off the SOP |
| Post anything | `@a007mr/posthero` — schedules and publishes to LinkedIn, X, Instagram, Facebook, YouTube, TikTok, Threads, Bluesky | **DENIED — posts.** Eight send paths in one skill |

### VP Retreats · Retreat Producer

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Read the **Retreat SOP** and **PIAB SOP** | `@byungkyu/notion-api-skill` | Shape only, read side |
| Run an event end to end | `@afrexai-cto/afrexai-event-planning` — vendors, logistics, budgeting, timelines, staffing | Shape only. Its pricing half is **refused** outright: prices come off [offers.md](../offers.md) |
| A venue and equipment readiness check | `@golngod/training-checklist` — venue, hotel, equipment, materials, complete / short / not started | Shape only, and a genuinely good checklist shape. There is nothing to run it on: no retreat date, guest list, or venue is recorded |
| A guest intake form | — | **Not confirmed on ClawHub — named missing.** The dietary, rooming, arrival, AV, and incident fields stay blank; [blank-guest-intake](../../skills/blank-guest-intake/SKILL.md) is the skill that keeps them blank |

## The twenty-three unassigned craft seats

No new ClawHub search was run for these seats. A row below either reuses a `@owner/slug` already recorded above, or says **not confirmed on ClawHub — named missing**. Nothing here gets installed. Every one of these seats is unassigned: installing something does not staff a seat, name an account, invent a speaking date, or claim a wiki exists.

Same order as [desks/README.md](../desks/README.md).

### Senior Digital Designer — unassigned · Junior Digital Designer — unassigned · Senior Print and Book Designer — unassigned · Junior Print and Book Designer — unassigned

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Brand rules, a palette, a template | — | **Not confirmed on ClawHub — named missing.** `styleguide-os` is a locked program repo, not a source. The seats are unassigned |

### Social Media Strategist — unassigned · Social Media Account Expert — unassigned

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Post, schedule, or publish | `@a007mr/posthero` | **DENIED — posts.** Eight send paths in one skill. Which accounts exist is named missing, and the seats are unassigned |

### Book Strategist — unassigned · Book Writer — unassigned · Book Conceptual Editor — unassigned · Book Copy Writer — unassigned · Book Technical Editor — unassigned · Book Reader — unassigned

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| A book launch kit | `@charlie-morrison/book-launch-coach`, `@jinhuadeng/book-launch-campaign-kit` | **Refused.** Both generate positioning, copy, and promo assets from templates. Already refused on VP Campaigns. The bench is unassigned and no book is recorded |
| Write the words | `@ivangdavila/writing`, `@tangentus/editor-in-chief` | **Shape only**, and still not installed. The seats are unassigned. See the cross-seat writing note below |

### Persona Architect — unassigned

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| A persona or ICP | — | **Not confirmed on ClawHub — named missing.** The seat is unassigned, no sourced material is in hand, and this is not Anthony's COO / Chief Persona Architect title |

### Strategist — unassigned · Copy Writer — unassigned · Sales Writer — unassigned · Copy Editor — unassigned · Sales Editor — unassigned

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Write or edit copy | `@ivangdavila/writing`, `@tangentus/editor-in-chief`, `@poemswe/clarity-and-grace`, `@nubzparmesan/minnow-writing`, `@conorbronsdon/avoid-ai-writing` | **Shape only**, already named in the cross-seat note. Still not installed. The seats are unassigned |
| Send the draft | `@officialdelta/gmail-secretary` is the only Gmail skill above that promises not to auto-send; `@porteden/gmail-cli` and `@hith3sh/gmail-email` send | **DENIED** on every send, reply, and forward. No send without Michael |

### SEO Expert — unassigned

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Keywords, rankings, a site | — | **Not confirmed on ClawHub — named missing.** No site, analytics, or keyword list is recorded. The seat is unassigned |

### PR and Media — unassigned

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| A pitch that leaves the building | `@porteden/gmail-cli`, `@hith3sh/gmail-email`, `@coreyhaines31/cold-email` | **DENIED — sends.** A pitch is a send. The seat is unassigned, and no outlet or contact is recorded |

### University Speaking Booker — unassigned · Association and Corporate Speaking Booker — unassigned

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| Put a date on the calendar | `@porteden/calendar-skill` | Shape only on read verbs; **DENIED** on create and update — no meeting gets made to fill a phase, and there is no speaking calendar in this repo |
| Contact a school or a host | `@coreyhaines31/cold-email` | **DENIED — sends.** Both seats are unassigned |

### Pendulum Wiki Researcher — unassigned

| Would reach for | On ClawHub | Verdict |
|---|---|---|
| A wiki, a URL, a platform | — | **Not confirmed on ClawHub — named missing.** Whether a Pendulum wiki exists at all is named missing. Installing a wiki is refused on the seat page |

## Cross-seat, and worth naming once

**Writing.** Any seat that drafts could reach for `@ivangdavila/writing`, `@tangentus/editor-in-chief`, `@poemswe/clarity-and-grace`, `@nubzparmesan/minnow-writing` ("write clearly, say the thing, stop"), or `@conorbronsdon/avoid-ai-writing`. **Shape only.** The last two are the closest public statements of the voice this handbook already uses, and reading them costs nothing. Installing them still counts as a registry install.

**Memory.** `@ivangdavila/memory` exists and does the obvious thing. **Refused** — [engine.md](../engine.md) writes no `MEMORY.md` and no daily memory log, because nothing has run and there is nothing remembered.

**The one that is almost this repo.** `@borodich/personal-os-onboarding` sets up a "Personal OS" through a fifteen-minute interview and writes `SOUL.md`, `USER.md`, `IDENTITY.md`, `AGENTS.md`, **and `MEMORY.md`**. That is the same five-file shape as [engine/workspaces/](workspaces/README.md), which is good confirmation that the shape is a real convention and not something we invented. It is also **refused**, for the fifth file: a memory written at setup time, before anything has happened, is exactly the artifact this engine will not ship.

## Leftovers

- Nothing on this page is installed, and nothing on it should be installed without Michael. If that ever changes, it changes on [locks.md](../locks.md) first, not here.
- The registry moves. A slug confirmed on 20 Aug 2026 can be renamed, transferred, or pulled by a scan. Re-check before quoting a row as current, and do not treat this page as a live index.
- The **Official** filter on ClawHub was not readable from here. If someone opens it in a browser and it changes any verdict above, that is worth writing down.
- The row for the registry itself is in [SOURCES.md](../../SOURCES.md).
