# Phase 0 Report

**Program: Grok Workforce Intelligence Upgrade v1 — Phase 0 only.** **Written: 25 Aug 2026, by a Cursor cloud agent on a VM.** **Sections 2–7 and 10–12 recut the same day** after the operator's local Qwen sit produced a filename-only public inventory of the pack. **Not last-gated.**

This page is docs only. It is one leftover file. **No Phase 1 work was done, nothing was installed, nothing was activated, no connector was changed, no machine was touched, and the original workforce pack was not modified** — it is not reachable from the machine this was written on. No last-gated leftover-seat plan is restamped, and no `grok-intelligence-upgrade-v1` scaffolding was created: everything in section 8 is a proposal.

Platformology LLC is the legal entity. **Promote a Book** and **Book Retreat** are DBAs of it — not two companies, and not SmarterVoice ([company-facts.md](../../company-facts.md)). **COO is first QC. PA last-gates** ([runtime-wiring.md](../../runtime-wiring.md), [leftover-write.md](../../leftover-write.md)). **KPI "Current" stays empty** — no figure, including 0. No holder, client, price, pipeline, close, manuscript, legal rule, accounting rule, or HR rule is created by this report. Named missing stays named ([SOURCES.md](../../../SOURCES.md)).

## 1. Status

**READY_FOR_REVIEW.**

Phase 0 could be written from the inputs supplied. The gaps that would have justified BLOCKED are all recorded as blockers in section 10 rather than used as a reason to refuse the report. **READY_FOR_REVIEW is not a completion claim.** It means the report is finished and honest enough for an independent reviewer to check — it does not mean Phase 0 passed, and it does not authorize Phase 1.

**The status did not change when the Qwen inventory arrived.** That sit made several findings firmer and added two blockers; it resolved none of the decisions in section 12, and it authorizes nothing.

### Label key — read this before any row below

Every factual conclusion on this page carries exactly one of four labels.

| Label | What it means here |
|---|---|
| **PROVEN** | Either (a) the claim is about a file in this repo and a reviewer can open the named path, or (b) a prior session supplied **all four** of command, timestamp, exit code, and an evidence-artifact SHA-256 |
| **SELF-REPORTED** | An operator or a document stated it. No independent artifact, scan, or hash exists. Not upgradable to PROVEN by repetition |
| **UNVERIFIED** | Not measured, not run, not readable from this writer, or **any one** of hash / timestamp / exit code / path was not supplied |
| **FAILED** | A check ran and did not pass, or a stated requirement is not met |

**Absence of evidence is never PASS.** No SHA-256, exit code, timestamp, count, agent ID, fixture ID, or score appears here unless it was supplied. Where a value was not supplied, this page writes UNVERIFIED instead of guessing it.

**This writer re-ran none of the office-Mac commands.** Every integrity, OpenClaw, Ollama, and Qwen row below is **reused operator evidence**, cited to the session it came from. No new hash is minted anywhere on this page.

**What a filename-only inventory can and cannot settle.** The operator's Qwen sit listed pack filenames; it did not open pack files. So it can show that **a name is present** and that **a name is absent**, and that is all. A present name does not prove the file's content, and an absent name does not prove the *concept* is absent — content answering to a name could sit inside a differently named file. Every Qwen-sourced row below says which of the two it is, and none of them is written as if the file had been read.

## 2. Environment Boundary

Three environments are in scope and they are **not** interchangeable. A claim proven in one is not proven in the others.

### E1 — This writer: a Cursor cloud agent VM

| Claim | Classification | Basis |
|---|---|---|
| This report was written by a Cursor cloud agent on a VM, from a checkout of `platformology/company-os` at `/workspace` | **PROVEN** | This VM; the repo and this file are the artifact a reviewer can open |
| This writer cannot see the office Mac. No path under `/Users/mdrew` exists on this VM | **PROVEN** | This VM: `/Users` does not exist |
| The workforce pack is not present in this repo or on this VM, so nothing about its current on-disk state can be checked from here | **PROVEN** | Repo-wide search for pack filenames returns nothing |
| Local execution against any company machine, from this writer: **disabled** | **PROVEN** | Cloud VM with no route to the office Mac. Owner instruction also forbids activating local execution |
| Credentials, tokens, and keys: **not inspected, and none is listed on this page** | **UNVERIFIED** | Deliberately not looked at. Unknown is the honest state |
| Grok Bot connectors and plugins | **UNVERIFIED** | Not observable from this VM and not fished for. Any integration visible to this Cursor agent is Cursor-side and is **not** evidence about Grok Bot |
| The original workforce pack was not modified by this writer | **PROVEN** | It is unreachable from here; no write path exists to it |

### E2 — The Grok cloud computer

| Claim | Classification | Basis |
|---|---|---|
| Shared Grok Bots share one cloud computer | **SELF-REPORTED** | Pack `RESEARCH_REPORT` / xAI documentation as previously summarized. **Neither is readable from this writer and neither was re-proven here** |
| 23 Grok Bot chats already exist, for the assigned / leftover-file / parked seats, and are retained | **SELF-REPORTED** | Prior operator statement, PR 141 packet section B. No exported audit or hash |
| The 23 unassigned craft seats have no Grok chat | **SELF-REPORTED** | Same source |
| No pack skills were imported into Grok Bot for this program | **SELF-REPORTED** | Same source. There is no forensic scan; the absence of a scan is not a clean scan |
| No pack, bundle, or fixture material has been uploaded to Grok by this program | **SELF-REPORTED** | Same source. Uploading the full pack is a live exposure risk — BLOCK-007 |

### E3 — The office Mac (prior operator / Qwen evidence, not this agent's run)

Everything in this block was recorded on 2026-08-25 in America/Denver by operator sessions and is reused here. **This writer did not observe any of it.** Labels follow the rule in section 1: PROVEN only where the session supplied command, timestamp, exit code, **and** an artifact hash.

| Item as recorded | Classification | Limitation |
|---|---|---|
| OpenClaw CLI at `/Users/mdrew/Company/Engine/bin/openclaw`, version `2026.7.1-2 (0790d9f)` | **UNVERIFIED** | Console record only; **no evidence artifact or hash was supplied** |
| `openclaw config validate` reported config valid | **UNVERIFIED** | Console record only; no artifact hash, no timestamp |
| 46 existing OpenClaw agents matching the 46 seat slugs; model on all listed `ollama/office-hand`; bindings 0 | **UNVERIFIED** | Console record only; no artifact hash, no timestamp, no exit code |
| Security audit: critical 0, warn 1 (`gateway.trusted_proxies_missing`) | **PROVEN** | Command, 14:09:36 MDT, exit 0, and artifact `openclaw-security-audit.json` hash-anchored in the PR 141 packet |
| Official `preflight.sh` passes with `Engine/bin` on PATH, exit 0 | **PROVEN** | Command, 14:10:04 MDT, exit 0, artifact `preflight.txt` hash-anchored in the PR 141 packet |
| MCP servers: `[]` | **UNVERIFIED** | Artifact `openclaw-mcp.json` is hash-anchored, but **command, timestamp, and exit code were not supplied** |
| 32 bundled plugins, all enabled | **UNVERIFIED** | Artifact `openclaw-plugins.json` is hash-anchored; command, timestamp, and exit code not supplied |
| Ollama 0.32.14; `qwen3.8:27b-q8_0` present; observed context 8192; listener `127.0.0.1:11434` | **UNVERIFIED** | Console record; the `09a`–`09e` evidence hashes exist but **their mapping to command and filename was not supplied**, and no exit code was supplied |
| Safe pack start of 32K context applied | **FAILED** | Not applied during that session. 64K was never tested — **UNVERIFIED** |
| Independent OS-user / gateway separation for finance, people, legal, production | **FAILED** | One gateway, one OS user, 46 agents sharing both. No separate OS users exist and none is invented here — BLOCK-005 |

#### E3a — the operator's local Qwen sit, 14:27:41–14:30:17

A second, later operator session on the same machine. **This writer did not run it, did not watch it, and cannot read its output files.**

| Item as recorded | Classification | Limitation |
|---|---|---|
| A local sit ran `ollama run --think=false qwen3.8:27b-q8_0` from 2026-08-25T14:27:41 to 14:30:17 America/Denver, exit 0 | **SELF-REPORTED** | Command, both timestamps, exit code, and two output paths were supplied. **No SHA-256 was supplied for either output file**, so this is not hash-anchored and does not meet the PROVEN bar — BLOCK-019 |
| Output files `phase0-qwen-draft.txt` and `phase0-public-inventory.txt`, under `/Users/mdrew/Company/Jobs/workforce-pack-evidence-2026-08-25` | **UNVERIFIED** as artifacts | Named by path only. Unreadable from this writer; no hash to anchor them |
| The sit produced a **filename-only public inventory** of the pack and did not open pack files | **SELF-REPORTED** | This is the ceiling on every Qwen-sourced row in sections 4–7 |
| The Qwen draft called the intelligence-layer schemas MISSING | **SELF-REPORTED** | A model's own draft agreeing with this report is **not corroboration**. What carries weight is the filename inventory underneath it, not the draft's conclusion |
| The Qwen draft claimed no activation occurred | **SELF-REPORTED** | **A writer stating that it did not activate anything is not proof that nothing was activated.** No independent scan exists, and this claim is not upgraded |
| Whether the sit was an approved local step | **SELF-REPORTED** | Reported by the operator as finished. This writer did not authorize it, request it, or take part in it |

**Local execution for Phase 1 is approval-only.** The owner has not enabled local execution for this writer, and this report does not ask for it. The 14:27–14:30 sit was an operator-run local step on the operator's own machine; it changes nothing about E1, where local execution stays disabled.

**One disagreement is named and not settled here.** [runtime-openclaw.md](../../runtime-openclaw.md) reads OpenClaw as a shape rather than an installed thing, and [locks.md](../../locks.md) reads "No local LLM until Michael says go," while the prior evidence records an installed OpenClaw gateway and a resident local model on the office Mac. **How those reconcile is the owner's call** — BLOCK-010. Nothing here lifts a lock or edits those pages.

## 3. Package Integrity Evidence

**Reused evidence only. This writer re-ran nothing and minted no hash.** Sources: the sanitized 2026-08-25 office-Mac evidence session carried in the PR 141 leftover packet ([PR 141](https://github.com/platformology/company-os/pull/141), branch `cursor/workforce-pack-deployment-evidence-faa8`, **not merged into `main` at the time this page was written**), and the operator's later Qwen sit at 14:27:41–14:30:17.

| # | Claim | Command | Timestamp (MDT) | Exit | Evidence artifact | Classification |
|---|---|---|---|---|---|---|
| P0-I1 | ZIP SHA-256 observed matches expected `d39a2cafacd6b44b7bd976871c7eac6271aa0ef696fc5382f57c3769b2f71975` | `shasum -a 256` on the ZIP | 2026-08-25 14:07:44 | 0 | `01-zip-sha256.txt`, sha256 `4266f5b41066e337053b74144f3675a80a44c1d14841d1d3b4f3ddd94338c2f9` | **PROVEN** |
| P0-I2 | `SHA256SUMS.txt` SHA-256 observed matches expected `7d02915d72134d2fa7175b6ab920f25d251b0d336af5d0664afce4d49f475cfc` | `shasum -a 256` on `SHA256SUMS.txt` | 2026-08-25 14:07:44 | 0 | `02-sha256sums-txt-sha256.txt`, sha256 `7ab60de4bad21573a4412486cbb9199699e1cfeab9c35b70f7c8ff51b8fcc4d1` | **PROVEN** |
| P0-I3 | 91 file checksums verified | `verify_checksums.mjs` | window 14:07:53–14:08:56 | 0 | hash-anchored in the PR 141 packet | **PROVEN** |
| P0-I4 | 46 unique seats; 47 text-only skills validated | `validate_pack.py` | window 14:07:53–14:08:56 | 0 | hash-anchored in the PR 141 packet | **PROVEN** |
| P0-I5 | Candidate-bundle materialization test passes | `test_materialize_candidate_bundle.py` | window 14:07:53–14:08:56 | 0 | hash-anchored in the PR 141 packet | **PROVEN** |
| P0-I6 | Planner test passes | `test_plan.py` | window 14:07:53–14:08:56 | 0 | hash-anchored in the PR 141 packet | **PROVEN** |
| P0-I7 | Install-policy test passes | `test_install_policy.mjs` | window 14:07:53–14:08:56 | 0 | hash-anchored in the PR 141 packet | **PROVEN** |
| P0-I8 | The pack's **current** on-disk state, at any moment after that window | — | — | — | — | **UNVERIFIED** |
| P0-I9 | The pack was still present on that machine at 14:27:41–14:30:17 and a filename-only inventory of it was taken | `ollama run --think=false qwen3.8:27b-q8_0` | 2026-08-25 14:27:41–14:30:17 | 0 | `phase0-public-inventory.txt`, `phase0-qwen-draft.txt` — **no SHA-256 supplied** | **SELF-REPORTED** |

**Limitations that travel with every row above.**

- P0-I3 through P0-I7 carry a **window**, not per-script start times. Each per-script timestamp is **UNVERIFIED**.
- These prove a **validated package**, not an installed one. Nothing here shows a skill placed on an agent, and the install-policy test is an allow-check, not an install.
- Integrity was proven on the office Mac at one moment on 2026-08-25. **This writer cannot re-verify it**, so the pack's state today is P0-I8: UNVERIFIED.
- **P0-I9 is not an integrity re-check.** No checksum was recomputed at 14:27–14:30, and a filename listing cannot detect a changed file. It narrows P0-I8 only to this: the pack still existed on that machine twenty minutes after the integrity window. Nothing about its bytes at that later moment is evidenced.
- No new hash is introduced on this page. Where the PR 141 packet holds a digest that the owner did not restate in the Phase 0 brief, this page cites the artifact filename and points at that packet rather than re-transcribing the digest.

## 4. Roster Reconciliation

Two independent records of the same roster, compared. They agree.

### Side A — the `seats.json` extract (prior session)

Extract timestamp `2026-08-25T14:09:36-06:00`; evidence `seats-summary.txt`, sha256 `73bc38eb86de888dce52765b90e52484eddaadc9897c20c79c654b3490e28a8e`.

**Classification: UNVERIFIED as an artifact** — a hash and a timestamp were supplied, but **no command and no exit code were**, so it does not meet the PROVEN bar set in section 1. Its *content* is cross-checkable against this repo, and that cross-check is below.

| Bucket | Count | Seats |
|---|---|---|
| assigned | 18 | pa, coo, cto, cfo, cmo, cso, cco, chro, controller, bookkeeper, people-ops, head-of-content, head-of-author-success, client-success, vp-campaigns, campaign-coordinator, vp-retreats, retreat-producer |
| leftover_only / no live job | 3 | head-of-demand, head-of-sales, sdr |
| parked | 2 | head-of-engineering, developer |
| unassigned craft | 23 | book-conceptual-editor through strategist |
| **Total** | **46** | |

**Only one holder is recorded: COO — Anthony C. Garcia.** Every other holder is null / not recorded, and this page names none.

### Side B — this repo (openable by any reviewer)

| Claim | Classification | Path |
|---|---|---|
| 46 seat pages exist | **PROVEN** | `handbook/seats/` — 46 pages plus a README |
| 44 leftover files exist: the 43 leftover-file employees plus the CTO leftover | **PROVEN** | `handbook/leftovers/` — plus a README and three named sub-leftovers |
| Head of Engineering and Developer have **no** leftover file — they stay parked | **PROVEN** | Absent from `handbook/leftovers/`; stated on [leftovers/README.md](../README.md) |
| Head of Demand, Head of Sales, SDR are leftover-file assigned with no live job | **PROVEN** | [leftovers/README.md](../README.md), "three charter seats with no job to run" |
| 23 craft seats stay UNASSIGNED | **PROVEN** | [leftovers/README.md](../README.md), "the twenty-three unassigned seats" |
| Who fills each seat except COO is **not recorded** | **PROVEN** | [SOURCES.md](../../../SOURCES.md) named missing; [people.md](../../people.md) |

### Side C — the Qwen public inventory, 14:27:41–14:30:17

A second reading of `seats.json`, taken at the status-count level during the operator's local sit. **Classification: SELF-REPORTED** — command, both timestamps, exit code, and output paths were supplied, but **no SHA-256 was**, so it is not hash-anchored.

| Bucket | Count |
|---|---|
| assigned | 18 |
| leftover_only | 3 |
| parked | 2 |
| unassigned | 23 |
| **Total** | **46** |

The same sit listed **47 skill files: `workforce-core-guardrails` plus 46 seat skill names.** That resolves what the 47 in P0-I4 is made of — **46 per-seat skills and one shared guardrails file, not 47 seat skills** — at filename level only. **SELF-REPORTED.** No skill file was opened, so nothing about any skill's content is evidenced.

### Reconciliation result

Three records now describe the same roster: this repo (openable), the `seats.json` extract (hashed, no command or exit), and the Qwen inventory (command, timestamps, exit 0, no hash). **They agree on every bucket.**

| Question | Answer | Classification |
|---|---|---|
| Do the three records agree on 46? | Yes. Side A's and Side C's 18 assigned = this repo's 17 assigned seats with a job to run **plus the CTO**, whose leftover is last-gated on `company-run.md` and is not one of the 43 | **PROVEN** on the repo side |
| Do they agree on holders? | Yes. COO only. **Side C reported statuses, not holders**, so it neither confirms nor contradicts this | **PROVEN** on the repo side |
| Do they agree on parked and no-live? | Yes. 2 parked, 3 leftover-only, in all three | **PROVEN** on the repo side |
| Any contradiction found? | None found | **PROVEN** on the repo side |
| Is either operator record independently authenticated? | No. The extract has a hash but no command or exit code; the Qwen inventory has a command, timestamps, and exit code but **no hash** | **UNVERIFIED** for both |

**Agreement between three unauthenticated readings is not authentication.** Two of the three came off the same machine in the same afternoon, and the repo is the only side a reviewer can open. The agreement is worth recording; it does not raise either operator record to PROVEN.

**CSO, CCO, and Pendulum remain definition-gated.** What those three mean is not recorded and is not invented here — BLOCK-002. A seat page, a body, a desk, a router, a pack, a plan, a pass, and a leftover existing for a seat **does not staff it, unpark it, or create a live job**.

## 5. Current Artifact Inventory

### In this repo — PROVEN, every count is an openable path

| Artifact set | Count | Path |
|---|---|---|
| Seat pages | 46 | `handbook/seats/` |
| Bodies (knowledge briefs) | 46 | `handbook/bodies/` |
| Desks (tools / sit-down packs) | 46 | `handbook/desks/` plus `BUILD.md` and `CONFLICTS.md` |
| Plans | 46 | `handbook/plans/` |
| Passes | 43 | `handbook/passes/` |
| Person packs | 43 | `handbook/packs/` |
| Pipelines | 43 | `handbook/pipelines/` |
| Maps | 9 | `handbook/maps/` |
| Leftover files | 44 | `handbook/leftovers/` |
| Skills | 72 directories, of which 61 are `run-*` routers | `skills/` |
| OpenClaw workspace scaffolds | 23 | `handbook/engine/workspaces/` |
| Review gates | 2 | `reviews/` — `last-gate-checklist.md`, `README.md` |
| Source register | 1 | [SOURCES.md](../../../SOURCES.md), including its **Named missing** list |

### In the workforce pack — counts reused from operator evidence, contents not readable here

| Artifact set | Count | Classification |
|---|---|---|
| Seats in `seats.json` | 46 | **PROVEN** via P0-I4; statuses re-listed at 14:27–14:30 — **SELF-REPORTED** |
| Text-only skills | 47 | **PROVEN** via P0-I4. Composition, at filename level: `workforce-core-guardrails` plus 46 seat skill names — **SELF-REPORTED** via P0-I9 |
| Checksummed files | 91 | **PROVEN** via P0-I3 |
| Public validator scripts | 4 (`validate_pack.py`, `test_plan.py`, `test_install_policy.mjs`, `test_materialize_candidate_bundle.py`) plus `verify_checksums.mjs` | **PROVEN** via P0-I3 – P0-I7 |
| `schemas/` directory | **absent**, and no filename in the pack contains "schema" | **SELF-REPORTED** via P0-I9 — filename level only |
| KB-* content files, for the 18 catalog IDs KB-AUTHORITY through KB-WIKI | **0 filename hits, 18 misses** | **SELF-REPORTED** via P0-I9 — see section 6 |
| `SOURCE_CATALOG.md`, `ORG_DESIGN_AUDIT.md`, `RESEARCH_REPORT` | named, **contents not readable from this writer** | **UNVERIFIED** |
| A hidden craft acceptance fixture file | present at filename level, **not opened**. Its path is not restated here | **SELF-REPORTED** that the name exists; **UNVERIFIED** as to anything inside it — see section 7 |
| Pack skills installed on any agent | 0 | **PROVEN** by the absence of any install action, per the PR 141 packet |
| Permanent Grok Bots activated by the pack | 0 | **SELF-REPORTED** |
| Acceptance runs executed | 0 | **PROVEN** by PR 141 section E — zero runs, and zero is not a pass |

### Paths

| | |
|---|---|
| **PACK_ROOT observed** | `/Users/mdrew/Documents/Codex/2026-06-29/you-are-in-coding-execution-mode/grokbot-openclaw-workforce-pack` — **PROVEN** from prior operator evidence as the path that session used. Not guessed, and **not** the same thing as UPGRADE_ROOT |
| **UPGRADE_ROOT** | **Not supplied by the owner. UNVERIFIED.** A sibling directory named `grok-intelligence-upgrade-v1`, next to the pack, is **proposed as a name only**. It was not created, and no file was written to it — BLOCK-001 |

## 6. Knowledge Readiness

**The catalog is a requirement, not proof of content.** `SOURCE_CATALOG.md` lives in the pack and is **not readable from this writer**, so each KB entry's catalog-stated subject, catalog-stated owner, version, effective date, freshness, and location are **UNVERIFIED** for every row below without exception. The "subject as named" column is derived from the KB identifier itself and is not a quotation from the catalog.

**Every one of the 18 catalog IDs is MISSING as pack content.** The Qwen public inventory matched filenames for KB-AUTHORITY through KB-WIKI and returned **0 hits and 18 misses**. That is a filename-level result — **SELF-REPORTED**, via P0-I9 — and it is the strongest thing said here about the pack: **no catalog ID is upgraded to AVAILABLE anywhere on this page.** A catalog entry is a requirement someone wrote down, not content someone wrote.

The "in this repo" column is a **different question with a different answer**, and the two do not merge. Where this repo holds real sourced company content on a subject, that is recorded as PARTIAL against **this repo** — never against the catalog ID, and never as evidence that the pack's requirement is met.

Readiness values used in the repo column: **PARTIAL** = this repo holds real, sourced company content on that subject, though not a knowledge base; **MISSING** = this repo records the subject as an unfilled hole.

| KB ID | Subject as named (not from the catalog) | As pack content | Nearest real company content in this repo | Repo readiness | Classification of the repo readiness call |
|---|---|---|---|---|---|
| KB-AUTHORITY | Legal entity and what may be said about it | **MISSING** | [company-facts.md](../../company-facts.md) — Platformology LLC, DBAs Promote a Book and Book Retreat, not SmarterVoice; [locks.md](../../locks.md) | PARTIAL | **PROVEN** (pages exist) |
| KB-STRATEGY | How the company makes and moves money | **MISSING** | [how-money-moves.md](../../how-money-moves.md) — the five jobs; [company-run.md](../../company-run.md) | PARTIAL | **PROVEN** |
| KB-PORTFOLIO | The offer ladder | **MISSING** | [offers.md](../../offers.md) — public price ladder, quote-both rule. **Membership price and the lead magnet's Offers row stay named missing; Platinum Major List has no public price** | PARTIAL | **PROVEN** |
| KB-POLICY | Never / ask-first permissions | **MISSING** | [locks.md](../../locks.md) | PARTIAL | **PROVEN** |
| KB-CLIENT | Client records | **MISSING** | [clients.md](../../clients.md). **0 Current clients on the 18 Aug 2026 extract; Hoffman is a question, not a fact; folder names are not clients** | PARTIAL | **PROVEN** |
| KB-AUTHOR | Author engagement and milestones | **MISSING** | No author-success SOP and no author milestone schedule are recorded ([SOURCES.md](../../../SOURCES.md)) | MISSING | **PROVEN** (recorded as a hole) |
| KB-EDITORIAL | House editorial standard | **MISSING** | **No house style guide, dictionary, or date format is recorded**, and no hand-off order among the editing seats | MISSING | **PROVEN** |
| KB-BRAND | Brand book and visual identity | **MISSING** | **No brand book, palette, type, or logo is recorded** | MISSING | **PROVEN** |
| KB-CAMPAIGN | Campaign process and QA | **MISSING** | The Campaign SOP lives in Notion and this repo does not restate it. **No campaign-QA SOP, no milestone list, schedule, or dated plan is recorded** | MISSING | **PROVEN** |
| KB-CRM | Customer record system | **MISSING** | **The CRM is Notion Clients. HubSpot is closed and there is no connector.** A link to the Notion Clients database is **not recorded in this repo** | MISSING | **PROVEN** |
| KB-SERVICE | Client service and retention | **MISSING** | **No client-risk model, no NPS survey, and no referral log are recorded** | MISSING | **PROVEN** |
| KB-FINANCE | Money boundary and close | **MISSING** | [how-money-moves.md](../../how-money-moves.md), [company-facts.md](../../company-facts.md) money boundary, Blue Sky stays off the LLC books. **June and July 2026 are not closed; no Bench savings total and no Bench connector** | PARTIAL | **PROVEN** |
| KB-PEOPLE | Roster, vendors, HR process | **MISSING** | [people.md](../../people.md) — staff and vendors, holders not recorded except COO. **No hiring, onboarding, or classification SOP; Jhana's Role and Bob's Role are named missing** | PARTIAL | **PROVEN** |
| KB-EVENT | Retreats | **MISSING** | The Retreat SOP and the blank guest intake live in Notion. **No sourced retreat date, guest list, or venue; no next retreat; PIAB cycle time unrecorded** | MISSING | **PROVEN** |
| KB-TECH | Runtime and production stack | **MISSING** | [runtime.md](../../runtime.md), [runtime-openclaw.md](../../runtime-openclaw.md), [runtime-wiring.md](../../runtime-wiring.md), [engine.md](../../engine.md). **The production stack is named missing** | PARTIAL | **PROVEN** |
| KB-DESIGN | Design briefs and production | **MISSING** | **No design brief, production stack, studio address, or print vendor is recorded** | MISSING | **PROVEN** |
| KB-RESEARCH | Decision basis and sourcing discipline | **MISSING** | [research-basis.md](../../research-basis.md), [SOURCES.md](../../../SOURCES.md) | PARTIAL | **PROVEN** |
| KB-WIKI | Pendulum wiki | **MISSING** | **No Pendulum wiki exists and no decision that one gets built is recorded** | MISSING | **PROVEN** |

**For all 18 rows:** the pack-content call is **SELF-REPORTED** at filename level — a KB file living under a name that does not carry its catalog ID would not have been matched, so "0 hits" is a naming result, not a proof that no such content exists anywhere in the pack; catalog-stated owner — **UNVERIFIED**; version, effective date, freshness, and canonical location — **UNVERIFIED**; whether the repo content in the fourth column would satisfy the pack's KB requirement — **UNVERIFIED**, because the requirement itself has not been read.

**The count that matters for Phase 1: 18 of 18 catalog IDs have no pack content file, and 10 of the 18 subjects are also holes in this repo.** The 8 PARTIAL subjects are handbook pages, not knowledge bases, and calling them one would be the upgrade this page refuses to make.

**KPI "Current" is empty across the board** and nothing in this report fills it — not a count, not a percentage, not a 0. **Named missing stays named**: live Uncovery script; membership price; PIAB cycle time; the lead magnet's Offers row; Jhana's Role; Bob's Role; vendor rate, term, and dates; production stack; studio address; the two unresolved Cornelia Choe Zoom URLs; Platinum Major List price; the uncollapsed track record (124 / 128 / 130–131); Hoffman's status; who fills each seat except COO; the campaign-QA SOP; the NPS survey; the referral log; the client-risk model; the onboarding SOP; June and July 2026 close; Bench savings total and connector; the next PA and the current PA's tenure end; the Notion Clients link. That list is [SOURCES.md](../../../SOURCES.md)'s, not this page's, and this page fills none of it.

## 7. Intelligence-Layer Gap Analysis

Fifteen named intelligence-layer components, assessed against (a) this repo, which a reviewer can open, and (b) the pack, which this writer cannot read but which was **listed at filename level** during the operator's Qwen sit.

**What changed with the Qwen inventory.** The five packet schemas were previously UNVERIFIED in the pack because nobody had looked. Somebody has now looked at the **names**: there is **no `schemas/` directory and no pack filename containing "schema"**. That moves those rows from "nobody looked" to **SELF-REPORTED absent at filename level** — a real strengthening, and still not the same as having read the pack.

| Component | In this repo | In the pack | Classification |
|---|---|---|---|
| `TASK_PACKET` schema | **Absent.** Repo-wide search finds no such schema | **No `schemas/` directory; no filename containing "schema"** | **SELF-REPORTED** absent at filename level; **PROVEN** absent from this repo |
| `TASK_STATE` schema | **Absent** | Same | **SELF-REPORTED** absent at filename level; **PROVEN** absent from this repo |
| `RESULT_PACKET` schema | **Absent** | Same | **SELF-REPORTED** absent at filename level; **PROVEN** absent from this repo |
| `HANDOFF_PACKET` schema | **Absent** | Same | **SELF-REPORTED** absent at filename level; **PROVEN** absent from this repo |
| `FAILURE_RECORD` schema | **Absent** | Same | **SELF-REPORTED** absent at filename level; **PROVEN** absent from this repo |
| Role-to-workflow map | **PARTIAL.** [seat-job-map.md](../../seat-job-map.md) plus 61 `run-*` routers map seats to jobs, but there is no packet-level workflow map | No such filename reported. The pack's 47 skill files are `workforce-core-guardrails` plus 46 seat names — a **naming** correspondence to seats, not a workflow map | **PROVEN** for what exists in this repo; **UNVERIFIED** for any map inside the pack |
| Source authority hierarchy | **PARTIAL.** [SOURCES.md](../../../SOURCES.md), [locks.md](../../locks.md), `desks/CONFLICTS.md`, and the "seat page wins" rule on [leftovers/README.md](../README.md) give a working precedence, but it is not written as one hierarchy. **Pendulum's place in it is unresolved** | `SOURCE_CATALOG.md` is named; **it was not opened**, so whether it states a hierarchy is unknown | **PROVEN** for what exists in this repo; **UNVERIFIED** for a single stated hierarchy |
| Candidate-visible training examples | **Absent** as a named, versioned set | Not reported as present by the filename inventory | **UNVERIFIED** in the pack — a name that was not reported is weaker evidence than a targeted match, and none was run for this; **PROVEN** absent from this repo |
| Near-miss examples | **Absent** | Same | **UNVERIFIED** in the pack; **PROVEN** absent from this repo |
| Deterministic public validators | **PARTIAL.** None in this repo; the pack's four validators plus the checksum verifier all exited 0 | Present and exercised | **PROVEN** that four public validators plus a checksum verifier pass; **PARTIAL** as an intelligence layer, because they validate the package, not a role's output |
| External evaluator separation | A hidden craft acceptance fixture file is **present at filename level and was not opened**; its path is not restated, quoted, requested, or reproduced anywhere on this page | The fixture name exists; the separation itself is designed, not demonstrated | **SELF-REPORTED** that the name is present; **UNVERIFIED** that separation held. **Not opening a file is not the same as proving nobody else opened it** |
| Correction ledger | **Absent** | Not reported as present | **UNVERIFIED** in the pack; **PROVEN** absent from this repo |
| Model-routing thresholds | **Absent.** No threshold, tier, or cutoff is recorded and none is invented here | Not reported as present | **UNVERIFIED** in the pack; **PROVEN** absent from this repo |
| Failure-recovery rules | **PARTIAL.** `skills/last-gate-then-stop`, `skills/check-locks`, and [reviews/last-gate-checklist.md](../../../reviews/last-gate-checklist.md) give a refuse-and-stop discipline, but there is no recovery rule for a failed run | `workforce-core-guardrails` is named and **was not opened**, so whether it carries recovery rules is unknown | **PROVEN** for what exists in this repo; **UNVERIFIED** for the pack |
| Tests for all 46 roles | **Absent** | Validation counted **23 craft acceptance fixtures and 92 role-qualified traps** — craft coverage only | **UNVERIFIED** for the other 23 roles. **23 fixtures is not 46 roles, and no role has three clean runs because zero runs were executed** |

**Three rows deserve care, because a filename inventory invites over-reading.**

- **The five schema rows are the strongest negative on this page**, because a targeted match was run for the concept and returned nothing under any name containing "schema". They are still SELF-REPORTED, not PROVEN: no hash anchors the inventory, and schema content could sit inside a file named something else.
- **The example, correction-ledger, and routing rows are weaker negatives.** The inventory did not report those names; no targeted match for them was reported either. Not-reported is not the same as searched-and-absent, so they stay UNVERIFIED for the pack.
- **`workforce-core-guardrails` and `SOURCE_CATALOG.md` are named but unopened.** Either could contain material bearing on failure recovery or source authority. Nothing on this page assumes they do, and nothing assumes they do not.

**The honest summary, unchanged in direction and firmer in evidence.** The pack brings package-level integrity, 46 seat skill names plus a shared guardrails file, and a candidate/evaluator split by design. **The working intelligence layer is not there**: no schema files under any schema-bearing name, no KB content files for any of the 18 catalog IDs, and nothing reported for the example sets, the correction ledger, or the routing thresholds. None of it is invented as present, and none of the absences is written as a pass.

## 8. Phase 1 Proposed File Plan

**Nothing below exists and nothing below was created.** This is a proposal for a sibling directory `grok-intelligence-upgrade-v1/` next to the pack, at an UPGRADE_ROOT the owner has not yet supplied (BLOCK-001). Creating any of it needs DEC-005.

Proposed directories: `schemas/ knowledge/ recipes/ routing/ examples/ corrections/ metrics/ handoffs/ reports/`.

**Writer and reviewer defaults, from [leftover-write.md](../../leftover-write.md) and [runtime-wiring.md](../../runtime-wiring.md).** The docs writer is Claude in GitHub as a docs pull request, with Qwen as the fallback writer only if Claude credit is out. **COO and CTO scope; COO is first QC; PA last-gates.** A Grok seat scopes, assigns, and first-QCs — **it does not write these files**. Assignments below are proposals, not assignments made by this report.

**Visibility rule, applied without exception: no evaluator-only file is ever handed to a Grok Bot as candidate-visible material.** Evaluator-only files are written and reviewed by the docs writer and the human gate, and are excluded from every candidate bundle.

### `schemas/`

| Proposed file | Purpose | Writer | Reviewer | Visibility | Required inputs | Acceptance test |
|---|---|---|---|---|---|---|
| `TASK_PACKET.schema.json` | Fixed input contract for one unit of seat work | Docs writer | CTO scope, COO first QC, PA last gate | Candidate-visible | Confirmed role slug list; source-authority hierarchy; the refusal rules on [locks.md](../../locks.md) | A public validator rejects a packet missing any required field and accepts the section 9 pilot packet |
| `TASK_STATE.schema.json` | In-flight state of one packet, including refused and blocked states | Docs writer | Same | Candidate-visible | `TASK_PACKET.schema.json` | Every state is reachable from a named prior state; no state means "silently dropped" |
| `RESULT_PACKET.schema.json` | Fixed output shape, with "not sourced" as a first-class valid result | Docs writer | Same | Candidate-visible | `TASK_PACKET.schema.json`; the named-missing discipline in [SOURCES.md](../../../SOURCES.md) | A result whose every field reads "not sourced" validates as well-formed and is not scored as a failure |
| `HANDOFF_PACKET.schema.json` | Seat-to-seat handoff, naming sender, receiver, and what is unresolved | Docs writer | Same | Candidate-visible | The handoffs already written in [runtime-wiring.md](../../runtime-wiring.md) | A handoff naming a parked or leftover-only receiver is rejected at validation |
| `FAILURE_RECORD.schema.json` | One record per refusal, failure, or blocked run | Docs writer | Same | Candidate-visible | `TASK_STATE.schema.json` | A refusal-on-lock and a run failure produce distinguishable records |
| `README.md` | Index of the five schemas and which are candidate-visible | Docs writer | Same | Candidate-visible | The five schemas | Every schema in the directory has a row; no row without a file |

### `knowledge/`

| Proposed file | Purpose | Writer | Reviewer | Visibility | Required inputs | Acceptance test |
|---|---|---|---|---|---|---|
| `KB_INDEX.md` | One row per KB-* with owner, canonical location, version, effective date, freshness | Docs writer | COO first QC, PA last gate | Candidate-visible | A readable `SOURCE_CATALOG.md`, which this writer does not have | No row invents an owner, a version, or a date; unknown reads UNVERIFIED |
| `KB_GAP_REGISTER.md` | The unfilled-content register, keyed to the named-missing list | Docs writer | Same | Candidate-visible | [SOURCES.md](../../../SOURCES.md) named missing; section 6 above | Every gap quotes the register it came from; no gap is invented and none is closed |
| `SOURCE_AUTHORITY.md` | The single stated precedence: repo, Notion, dated extract, and how ties break | Docs writer | CTO scope, COO first QC, PA last gate | Candidate-visible | [locks.md](../../locks.md), [SOURCES.md](../../../SOURCES.md), `desks/CONFLICTS.md`, [leftovers/README.md](../README.md) | Three recorded past conflicts resolve the same way by the written rule as they did in the repo |

### `recipes/`

| Proposed file | Purpose | Writer | Reviewer | Visibility | Required inputs | Acceptance test |
|---|---|---|---|---|---|---|
| `RECIPE_TEMPLATE.md` | The shape a workflow recipe takes — headings only, no content | Docs writer | COO first QC, PA last gate | Candidate-visible | The five schemas | The template contains no company fact of any kind |
| `book-conceptual-editor/<pilot-workflow>.md` | The one pilot workflow recipe from section 9 | Docs writer | CTO scope, COO first QC, PA last gate | Candidate-visible | DEC-004; owner-supplied fixture material; KB-AUTHOR and KB-EDITORIAL content that does not currently exist | The pilot produces a valid `RESULT_PACKET` on the supplied fixture, and refuses cleanly when the fixture is absent. **This recipe is not written in Phase 0** |

### `routing/`

| Proposed file | Purpose | Writer | Reviewer | Visibility | Required inputs | Acceptance test |
|---|---|---|---|---|---|---|
| `ROLE_WORKFLOW_MAP.md` | Role → workflow → recipe → required KB, for the roles in scope | Docs writer | CTO scope, COO first QC, PA last gate | Candidate-visible | [seat-job-map.md](../../seat-job-map.md); the `run-*` routers; the roster in section 4 | Parked and leftover-only seats appear with no live workflow; no seat is silently given one |
| `MODEL_ROUTING.md` | Which class of work goes to which model, and on what threshold | Docs writer | CTO scope, COO first QC, PA last gate | Candidate-visible | **Owner thresholds, which do not exist yet** | No threshold appears that the owner did not set; unset reads UNVERIFIED |
| `ESCALATION_AND_RECOVERY.md` | Failure-recovery rules and the refusal ladder — where an ask goes when a run cannot proceed | Docs writer | Same | Candidate-visible | `skills/last-gate-then-stop`, `skills/check-locks`, [reviews/last-gate-checklist.md](../../../reviews/last-gate-checklist.md) | Every failure class in `FAILURE_RECORD` has exactly one named destination, and none of them is "proceed anyway" |

### `examples/`

| Proposed file | Purpose | Writer | Reviewer | Visibility | Required inputs | Acceptance test |
|---|---|---|---|---|---|---|
| `EXAMPLES_POLICY.md` | What may be shown to a candidate seat, and what may never be | Docs writer | COO first QC, PA last gate | Candidate-visible | The visibility rule above | The policy names the evaluator-only class and forbids its distribution, without reproducing any of it |
| `candidate-visible/<role>/gold-01.md` | One worked example of a good result | Docs writer | CTO scope, COO first QC, PA last gate | Candidate-visible | Owner-supplied fixture material only — **no client, author, or manuscript** | The example validates against `RESULT_PACKET.schema.json` and contains no company fact that is not already sourced |
| `candidate-visible/<role>/near-miss-01.md` | One near-miss, with the single reason it misses | Docs writer | Same | Candidate-visible | The gold example | The stated reason is checkable against a schema field or a written rule, not a matter of taste |

### `corrections/`

| Proposed file | Purpose | Writer | Reviewer | Visibility | Required inputs | Acceptance test |
|---|---|---|---|---|---|---|
| `CORRECTION_LEDGER.csv` | One row per corrected output: what was wrong, what rule it broke, what changed | Docs writer | COO first QC, PA last gate | Candidate-visible | `FAILURE_RECORD.schema.json` | Every row cites a rule or schema field; a row with no cited rule fails validation |
| `CORRECTION_POLICY.md` | Who may correct, and what a correction may never do | Docs writer | CTO scope, COO first QC, PA last gate | Candidate-visible | [locks.md](../../locks.md) | The policy forbids a correction that invents a company fact to make an output pass |

### `metrics/`

| Proposed file | Purpose | Writer | Reviewer | Visibility | Required inputs | Acceptance test |
|---|---|---|---|---|---|---|
| `METRICS_DEFINITIONS.md` | What each Phase 1 measure counts and what it must never be read off | Docs writer | COO first QC, PA last gate | Candidate-visible | The KPI discipline in [SOURCES.md](../../../SOURCES.md) | **KPI Current stays empty** — the file defines names and leaves every current value empty, including 0 |
| `phase-1-run-log.csv` | One row per acceptance run actually executed | Docs writer | Same | Evaluator-only | Executed runs | An empty file is the honest state until a run happens, and an empty file is never reported as a pass |

### `handoffs/`

| Proposed file | Purpose | Writer | Reviewer | Visibility | Required inputs | Acceptance test |
|---|---|---|---|---|---|---|
| `HANDOFF_REGISTER.md` | Which seat hands what to which seat, sourced not invented | Docs writer | CTO scope, COO first QC, PA last gate | Candidate-visible | [runtime-wiring.md](../../runtime-wiring.md); `desks/CONFLICTS.md` | Every handoff cites the page that already records it; **the unrecorded hand-off order among the editing seats stays recorded as unrecorded** |

### `reports/`

| Proposed file | Purpose | Writer | Reviewer | Visibility | Required inputs | Acceptance test |
|---|---|---|---|---|---|---|
| `PHASE_1_REPORT.md` | The Phase 1 equivalent of this page, same labeling discipline | Docs writer | COO first QC, PA last gate | Candidate-visible | Phase 1 work actually performed | Every conclusion carries exactly one of the four labels; absence is never PASS |
| `evaluator-only/EVALUATOR_SEPARATION.md` | How evaluator material is kept out of every candidate bundle, and how a leak would be detected | Docs writer | CTO scope, COO first QC, PA last gate | **Evaluator-only — never handed to a Grok Bot** | The separation design | The file states the rule without reproducing, quoting, or pointing to any hidden fixture content, and a candidate bundle built under it contains none of it |

**Two things this plan does not do.** It does not upload the pack, any bundle, or any fixture to Grok. It does not assign an evaluator-only file to a Grok seat in any capacity, candidate-visible or otherwise.

## 9. Pilot Recommendation

**Recommended pilot role: `book-conceptual-editor`. Exactly one narrow workflow. The recipe is not written here.**

| | |
|---|---|
| **Workflow** | A single-excerpt structural read that returns one fixed-shape `RESULT_PACKET`, run against an owner-supplied evaluation excerpt |
| **Scope limit** | One excerpt, one packet, one pass. No second workflow, no queue, no batch |
| **What it is** | A capability exercise on supplied material |
| **What it is not** | A live job, a staffing decision, a deliverable to any author, or evidence the seat is filled |

**Why this role is the right pilot.**

- It is one of the 23 **unassigned craft** seats, so a pilot cannot be mistaken for live client work — **PROVEN** ([leftovers/README.md](../README.md)).
- It is **capability-built, not pipeline-built**: it needs no CRM record, no campaign, no forecast, and no money figure, so nothing about a pipeline has to be invented to exercise it — **PROVEN** from the seat's own leftover and plan.
- **It has no live job to disturb.** Its recorded leftover is the vacancy plus the named holes — **PROVEN**.
- It sits inside the pack's evidenced test coverage class: the prior validation counted 23 craft acceptance fixtures, and this is a craft seat — **PROVEN** via P0-I4. Whether a fixture exists for *this* seat specifically is **UNVERIFIED**, because the fixture set was not opened.

**Required sources: KB-AUTHOR and KB-EDITORIAL. Both are missing.**

| Required input | State | Classification |
|---|---|---|
| KB-AUTHOR content | Missing on both sides: no author-success SOP and no author milestone schedule in this repo, and **no KB-AUTHOR content file in the pack** (0 of 18 filename hits) | **MISSING** — **PROVEN** as a recorded hole in the repo; **SELF-REPORTED** for the pack |
| KB-EDITORIAL content | Missing on both sides: no house style guide, dictionary, or date format in this repo, and **no KB-EDITORIAL content file in the pack** | **MISSING** — **PROVEN** as a recorded hole in the repo; **SELF-REPORTED** for the pack |
| An excerpt to read | **No manuscript, author, or engagement exists**, and none is invented here. The pilot needs owner-supplied evaluation material | **MISSING** |
| A fixture for this seat in the pack | Not opened, not requested. The fixture file's name is present; whether it covers this seat is unknown | **UNVERIFIED** |
| A `RESULT_PACKET` shape for the pilot to return | **No schema exists** under any schema-bearing filename in the pack, and none exists in this repo. Phase 1 would have to write it first | **SELF-REPORTED** absent from the pack; **PROVEN** absent from this repo |

**Missing company decisions, carried as blockers rather than answered.**

- **BLOCK-011.** The seat's own leftover says in as many words: do not write an edit letter, a structural diagnosis, a reverse outline, or revision notes, and do not invent a manuscript or an author. A capability exercise on owner-supplied material is arguably a different thing from live seat work — **but this report does not decide that**, and the pilot does not start until the owner does (DEC-004).
- **BLOCK-012.** The hand-off order among the three editing seats is not recorded, so where a pilot result would go next is unknown.
- **BLOCK-013.** Who fills this seat is not recorded, and a pilot does not fill it, staff it, or change its UNASSIGNED state.

**Until DEC-004 and the two missing knowledge bases are supplied, the pilot cannot run.** Naming the pilot is not starting it.

## 10. Risks and Blockers

Stable IDs. These do not get renumbered in later phases; a resolved blocker keeps its ID and is marked resolved.

| ID | Blocker | Classification | Why it matters for Phase 1 |
|---|---|---|---|
| **BLOCK-001** | **UPGRADE_ROOT is unspecified.** The owner supplied no path; `grok-intelligence-upgrade-v1` is a proposed sibling **name only** and was not created | **UNVERIFIED** | Nothing in section 8 can be written anywhere until a root is named. Guessing a root risks writing into the pack |
| **BLOCK-002** | **CSO, CCO, and Pendulum are definition-gated.** What each means is not recorded | **UNVERIFIED** | Any workflow, KB mapping, or routing rule touching those three would invent a meaning. They stay gated unless the owner defines them |
| **BLOCK-003** | **Head of Engineering and Developer are parked** | **PROVEN** ([locks.md](../../locks.md), [leftovers/README.md](../README.md)) | No Phase 1 artifact activates, unparks, or gives either a workflow |
| **BLOCK-004** | **Head of Demand, Head of Sales, and SDR are leftover-file assigned with no live job** | **PROVEN** | They get no live workflow, no pipeline, no forecast, and no lead volume in Phase 1 |
| **BLOCK-005** | **No OS-user separation.** One gateway, one OS user, 46 agents sharing both; finance, people, legal, and production are not independent boundaries | **FAILED** | An intelligence layer that assumes separated boundaries would be assuming something that does not hold |
| **BLOCK-006** | **`clawhub` is eligible in the skill inventory and is not to be installed** | **UNVERIFIED** as to current state; the not-to-install instruction is the owner's | Phase 1 installs nothing. This is recorded so no later step reads eligibility as approval |
| **BLOCK-007** | **Hidden-oracle exposure if the pack is uploaded to Grok.** The pack contains a hidden craft acceptance fixture file; uploading the full pack to a shared Grok cloud computer would put evaluator material in front of candidate seats | **UNVERIFIED** — no upload is evidenced either way | **Do not upload the full pack.** This report does not open, quote, name, or request that file |
| **BLOCK-008** | **The 32K safe-start context was not applied**; observed context was 8192 and 64K was never tested | **FAILED** for 32K; **UNVERIFIED** for 64K | Any Phase 1 workload sizing based on a 32K assumption would be unfounded |
| **BLOCK-009** | **Zero acceptance runs have been executed.** No role has three clean runs and no role is activation-ready | **PROVEN** by the PR 141 packet | There is no baseline to measure a Phase 1 improvement against. Zero runs is not a pass |
| **BLOCK-010** | **This handbook and the live evidence disagree** about whether OpenClaw and a local model are installed on the office Mac | **UNVERIFIED** — the conflict is real; the resolution is not recorded | **This is the owner's to settle, not this report's.** Nothing here edits those pages or lifts a lock |
| **BLOCK-011** | The pilot seat's leftover forbids producing an edit letter, structural diagnosis, reverse outline, or revision notes; whether a capability exercise on supplied material is exempt is not recorded | **PROVEN** as a recorded instruction; the exemption question is **UNVERIFIED** | The pilot cannot start until the owner decides (DEC-004) |
| **BLOCK-012** | The hand-off order among the three editing seats is not recorded | **PROVEN** as a recorded hole | A `HANDOFF_PACKET` for the pilot has no recorded destination |
| **BLOCK-013** | Who fills any seat except COO is not recorded | **PROVEN** | No Phase 1 artifact names a holder, and no pilot staffs a seat |
| **BLOCK-014** | **The five packet schemas do not exist under any schema-bearing filename in the pack**, and the example sets, correction ledger, and routing thresholds are not reported present anywhere | **PROVEN** absent from this repo; **SELF-REPORTED** absent from the pack at filename level for the schemas; **UNVERIFIED** in the pack for the rest | This is the substance of the upgrade, and the Qwen inventory makes it firmer: it is unbuilt, not merely unlooked-at |
| **BLOCK-015** | **Test coverage is craft-only.** 23 craft fixtures and 92 traps were validated; coverage for the other 23 roles is not evidenced | **UNVERIFIED** | "Tests for all 46 roles" is not supported by anything supplied |
| **BLOCK-016** | **No KB-* catalog ID has a pack content file — 0 hits, 18 misses** — and 10 of the 18 subjects are also holes in this repo | **SELF-REPORTED** for the pack side at filename level; **PROVEN** for the repo side | A knowledge layer built on empty knowledge bases would have to invent the content, which is forbidden. The 8 PARTIAL subjects are handbook pages, not knowledge bases |
| **BLOCK-017** | **This writer cannot verify the pack's current state.** Integrity is proven only for the 14:07–14:08 window; the 14:27–14:30 sit listed filenames and **recomputed no checksum** | **UNVERIFIED** | Phase 1 should re-verify integrity at the machine that holds the pack before anything is built beside it. A filename listing cannot detect a changed file |
| **BLOCK-018** | **Grok connectors and plugins are unknown**, and credentials were deliberately not inspected | **UNVERIFIED** | Recorded so no later step treats unknown as "none". This report does not ask for either |
| **BLOCK-019** | **The Qwen sit's two evidence files carry no SHA-256.** Command, both timestamps, exit 0, and paths were supplied; a hash was not | **SELF-REPORTED** | Everything sections 4–7 take from that inventory is capped at SELF-REPORTED because of this one gap. A hash for the two files would raise the whole inventory — DEC-008 |
| **BLOCK-020** | **A filename inventory cannot answer content questions.** `workforce-core-guardrails` and `SOURCE_CATALOG.md` are named and unopened, so whether they carry recovery rules or a source-authority hierarchy is unknown | **UNVERIFIED** | Phase 1 would be building `ESCALATION_AND_RECOVERY.md` and `SOURCE_AUTHORITY.md` beside two pack files that might already answer part of the question |

## 11. Claims Ledger

| claim_id | claim | classification | evidence_reference | originating_machine | timestamp | limitations |
|---|---|---|---|---|---|---|
| C-001 | ZIP SHA-256 observed matches expected `d39a2ca…f71975` | PROVEN | `01-zip-sha256.txt`, sha256 `4266f5b…38c2f9`; `shasum -a 256`; exit 0 | Office Mac | 2026-08-25 14:07:44 MDT | Reused prior evidence; this writer did not re-run it |
| C-002 | `SHA256SUMS.txt` SHA-256 observed matches expected `7d02915…75cfc` | PROVEN | `02-sha256sums-txt-sha256.txt`, sha256 `7ab60de…8fcc4d1`; exit 0 | Office Mac | 2026-08-25 14:07:44 MDT | Same |
| C-003 | 91 file checksums verified, exit 0 | PROVEN | `verify_checksums.mjs`; artifact hash-anchored in the PR 141 packet | Office Mac | window 14:07:53–14:08:56 MDT | Per-script start time UNVERIFIED |
| C-004 | 46 seats and 47 text-only skills validated, exit 0 | PROVEN | `validate_pack.py`; artifact hash-anchored in the PR 141 packet | Office Mac | window 14:07:53–14:08:56 MDT | Validates the package, not an install |
| C-005 | `test_materialize_candidate_bundle.py`, `test_plan.py`, `test_install_policy.mjs` all exit 0 | PROVEN | Artifacts hash-anchored in the PR 141 packet | Office Mac | window 14:07:53–14:08:56 MDT | Allow-checks, not installs |
| C-006 | The pack's current on-disk state | UNVERIFIED | none | not supplied | not supplied | Pack unreachable from this writer |
| C-007 | PACK_ROOT is `/Users/mdrew/Documents/Codex/2026-06-29/you-are-in-coding-execution-mode/grokbot-openclaw-workforce-pack` | PROVEN | Prior operator evidence session, PR 141 packet | Office Mac | 2026-08-25 | Owner has not re-confirmed it for this program — DEC-001 |
| C-008 | UPGRADE_ROOT | UNVERIFIED | none | not supplied | not supplied | Not supplied; sibling name proposed only; nothing created |
| C-009 | 46 seats; only recorded holder is COO, Anthony C. Garcia | PROVEN | `handbook/seats/` (46 pages) and [SOURCES.md](../../../SOURCES.md) named missing, openable in this repo | This VM (repo) | 25 Aug 2026 | Repo-side proof; the `seats.json` extract is C-010 |
| C-010 | The `seats.json` extract records the same roster | UNVERIFIED | `seats-summary.txt`, sha256 `73bc38e…e28a8e` | Office Mac | 2026-08-25T14:09:36-06:00 | Hash and timestamp supplied; **command and exit code were not** |
| C-011 | 18 assigned / 3 leftover-only / 2 parked / 23 unassigned craft, summing to 46, and all three records agree | PROVEN | [leftovers/README.md](../README.md); `handbook/leftovers/` file set; corroborated by C-010 and C-044 | This VM (repo) | 25 Aug 2026 | Agreement is on content. Neither operator record is authenticated, and three unauthenticated readings agreeing is not authentication |
| C-012 | Head of Engineering and Developer are parked and have no leftover file | PROVEN | [locks.md](../../locks.md); absence from `handbook/leftovers/` | This VM (repo) | 25 Aug 2026 | — |
| C-013 | CSO, CCO, and Pendulum meanings are unresolved | UNVERIFIED | PR 141 unresolved-blocker list; no repo page defines them | Office Mac / this VM | 25 Aug 2026 | Not invented here |
| C-014 | This repo holds 46 seats, 46 bodies, 46 desks, 46 plans, 43 passes, 43 packs, 43 pipelines, 9 maps, 44 leftovers, 72 skills, 23 workspace scaffolds | PROVEN | Directory listings, all openable | This VM (repo) | 25 Aug 2026 | Counts as of this commit |
| C-015 | No `TASK_PACKET`, `TASK_STATE`, `RESULT_PACKET`, `HANDOFF_PACKET`, or `FAILURE_RECORD` schema exists in this repo | PROVEN | Repo-wide search returns no match | This VM (repo) | 25 Aug 2026 | Says nothing about the pack — that is C-016 |
| C-016 | The pack has no `schemas/` directory and no filename containing "schema", so none of the five exists under a schema-bearing name | SELF-REPORTED | `phase0-public-inventory.txt` — filename match, **no hash supplied** | Office Mac | 2026-08-25 14:27:41–14:30:17 MDT | Filename level only. Schema content inside a differently named, unopened file would not have been caught |
| C-017 | Four public validators plus a checksum verifier exist and passed | PROVEN | C-003 – C-005 | Office Mac | 2026-08-25 | Package-level, not role-output-level. PARTIAL as an intelligence layer |
| C-018 | A hidden craft acceptance fixture file is present at filename level and was not opened | SELF-REPORTED | Operator statement plus the filename inventory; the path is not restated, quoted, or requested here | Office Mac | 2026-08-25 14:27:41–14:30:17 MDT | Presence of the name only. **Not opening it is not proof that nobody else did, and not proof that separation held** |
| C-019 | Evaluator separation is demonstrated | UNVERIFIED | none | not supplied | not supplied | PARTIAL by design at best; no forensic scan exists |
| C-020 | 23 craft acceptance fixtures and 92 role-qualified traps were validated | PROVEN | `validate_pack.py`, C-004 | Office Mac | window 14:07:53–14:08:56 MDT | Craft coverage only; the other 23 roles are C-021 |
| C-021 | Tests exist for all 46 roles | UNVERIFIED | none | not supplied | not supplied | 23 fixtures is not 46 roles |
| C-022 | Zero acceptance runs have been executed; no role has three clean runs | PROVEN | PR 141 packet section E | Office Mac | 2026-08-25 | Zero is the honest result and is not a pass |
| C-023 | Security audit: critical 0, warn 1, exit 0 | PROVEN | `openclaw-security-audit.json`, hash-anchored in the PR 141 packet | Office Mac | 2026-08-25 14:09:36 MDT | Warning is `gateway.trusted_proxies_missing` |
| C-024 | Official preflight passes with `Engine/bin` on PATH, exit 0 | PROVEN | `preflight.txt`, hash-anchored in the PR 141 packet | Office Mac | 2026-08-25 14:10:04 MDT | Depends on a PATH that is not the default |
| C-025 | OpenClaw version, config validity, 46 agents, model tag, bindings 0 | UNVERIFIED | Console records with no artifact hash supplied | Office Mac | partly not supplied | Downgraded from the prior packet's console-record label, per the rule in section 1 |
| C-026 | MCP servers `[]`; 32 bundled plugins enabled | UNVERIFIED | Artifacts hash-anchored, but command, timestamp, and exit code not supplied | Office Mac | not supplied | Artifact exists; the run around it does not meet the PROVEN bar |
| C-027 | Ollama 0.32.14, `qwen3.8:27b-q8_0` present, observed context 8192, listener `127.0.0.1:11434` | UNVERIFIED | Evidence labels `09a`–`09e` exist; their mapping to commands and filenames was not supplied | Office Mac | 2026-08-25 14:07:55 MDT | No exit code supplied for any command in that block |
| C-028 | The 32K safe-start context was not applied | FAILED | Prior evidence: observed context 8192 | Office Mac | 2026-08-25 | 64K never tested — UNVERIFIED |
| C-029 | Independent OS-user / gateway separation | FAILED | One gateway, one OS user, 46 agents; PR 141 section C10 | Office Mac | 2026-08-25 | No separate OS users invented here |
| C-030 | Shared Grok Bots share one cloud computer | SELF-REPORTED | Pack `RESEARCH_REPORT` / xAI documentation as previously summarized | Grok cloud computer | not supplied | Neither document is readable from this writer; not re-proven |
| C-031 | 23 Grok chats already exist and are retained; the 23 craft seats have none | SELF-REPORTED | Prior operator statement, PR 141 section B | Grok cloud computer | 2026-08-25 | No exported audit, no hash |
| C-032 | No pack skills were imported into Grok for this program | SELF-REPORTED | Prior operator statement | Grok cloud computer | 2026-08-25 | Absence of a scan is not a clean scan |
| C-033 | Grok connectors and plugins | UNVERIFIED | Not observable from this VM; not fished for | Cursor cloud agent VM | 25 Aug 2026 | Cursor-side integrations are not evidence about Grok |
| C-034 | Credentials | UNVERIFIED | Deliberately not inspected | Cursor cloud agent VM | 25 Aug 2026 | None is listed anywhere on this page |
| C-035 | Local execution from this writer is disabled | PROVEN | Cloud VM; `/Users` does not exist here | Cursor cloud agent VM | 25 Aug 2026 | Local execution for Phase 1 stays approval-only |
| C-036 | The original workforce pack was not modified | PROVEN | Unreachable from this writer; no write path exists to it | Cursor cloud agent VM | 25 Aug 2026 | — |
| C-037 | 10 of the 18 KB-* subjects have no approved company content in this repo; 8 are partial | PROVEN | Section 6, every row citing an openable path or a recorded hole | This VM (repo) | 25 Aug 2026 | A PARTIAL handbook page is not a knowledge base, and no catalog ID is upgraded to AVAILABLE on the strength of one |
| C-038 | KB-* catalog owner, version, effective date, freshness, and location | UNVERIFIED | `SOURCE_CATALOG.md` not readable from this writer | not supplied | not supplied | The catalog is a requirement, not proof of content |
| C-039 | KPI "Current" is empty and no figure, including 0, is written here | PROVEN | [SOURCES.md](../../../SOURCES.md) named missing; this page writes none | This VM (repo) | 25 Aug 2026 | — |
| C-040 | No `grok-intelligence-upgrade-v1` file, directory, or scaffold was created | PROVEN | This pull request adds exactly one file, this page | Cursor cloud agent VM | 25 Aug 2026 | Section 8 is a proposal only |
| C-041 | No employee was activated, nothing was installed, no connector changed, nothing merged, no last-gated plan restamped | PROVEN | The diff of this pull request | Cursor cloud agent VM | 25 Aug 2026 | Verifiable by reading the diff |
| C-042 | The handbook and the live evidence disagree about OpenClaw and a local model on the office Mac | UNVERIFIED | [runtime-openclaw.md](../../runtime-openclaw.md), [locks.md](../../locks.md) versus the prior evidence session | This VM (repo) / Office Mac | 25 Aug 2026 | The conflict is recorded; the resolution is the owner's — BLOCK-010. The 14:27–14:30 local model sit is one more fact on the evidence side of it and settles nothing |
| C-043 | A local sit ran `ollama run --think=false qwen3.8:27b-q8_0`, exit 0, writing `phase0-qwen-draft.txt` and `phase0-public-inventory.txt` | SELF-REPORTED | Both filenames supplied under `/Users/mdrew/Company/Jobs/workforce-pack-evidence-2026-08-25`; **no SHA-256 for either** | Office Mac | 2026-08-25T14:27:41 to 14:30:17 America/Denver | Command, timestamps, exit code, and paths supplied; the missing hash caps everything drawn from it — BLOCK-019 |
| C-044 | `seats.json` statuses re-listed: assigned 18, leftover_only 3, parked 2, unassigned 23, total 46 | SELF-REPORTED | `phase0-public-inventory.txt` | Office Mac | 2026-08-25 14:27:41–14:30:17 MDT | Statuses only. **No holder was read**, so this neither confirms nor contradicts the COO-only holder record |
| C-045 | The pack holds 47 skill files: `workforce-core-guardrails` plus 46 seat skill names | SELF-REPORTED | `phase0-public-inventory.txt` | Office Mac | 2026-08-25 14:27:41–14:30:17 MDT | Filename level. Resolves what P0-I4's 47 is made of; says nothing about any skill's content, quality, or fitness |
| C-046 | No KB content file matches any of the 18 catalog IDs KB-AUTHORITY through KB-WIKI — 0 hits, 18 misses | SELF-REPORTED | `phase0-public-inventory.txt` | Office Mac | 2026-08-25 14:27:41–14:30:17 MDT | Filename match only. A KB file named without its catalog ID would not have matched |
| C-047 | Every one of the 18 catalog IDs is MISSING as pack content | SELF-REPORTED | C-046 | Office Mac | 2026-08-25 14:27:41–14:30:17 MDT | **No catalog ID is upgraded to AVAILABLE anywhere on this page**, and the repo's 8 PARTIAL subjects are a separate finding that does not transfer |
| C-048 | The Qwen draft called the intelligence-layer schemas MISSING | SELF-REPORTED | `phase0-qwen-draft.txt` | Office Mac | 2026-08-25 14:27:41–14:30:17 MDT | **A model's draft agreeing with this report is not corroboration.** The weight sits in C-016's filename match, not in the draft |
| C-049 | The Qwen draft claimed no activation occurred | SELF-REPORTED | `phase0-qwen-draft.txt` | Office Mac | 2026-08-25 14:27:41–14:30:17 MDT | **A writer's statement that it did not activate anything is not proof that nothing was activated.** No independent scan exists, and this is not upgraded |
| C-050 | The pack was still present on that machine at 14:27–14:30 | SELF-REPORTED | An inventory of it was taken | Office Mac | 2026-08-25 14:27:41–14:30:17 MDT | **Not an integrity re-check.** No checksum was recomputed; a filename listing cannot detect a changed file |
| C-051 | `workforce-core-guardrails` and `SOURCE_CATALOG.md` are named in the pack and were not opened | SELF-REPORTED | `phase0-public-inventory.txt` | Office Mac | 2026-08-25 14:27:41–14:30:17 MDT | Either could bear on failure recovery or source authority. Nothing here assumes they do or do not — BLOCK-020 |

## 12. Requested Decisions

Only decisions required before Phase 1 can start. **No credential, no local-execution enablement, no connector change, and no evaluator material is requested here.**

| ID | Decision requested | Why it blocks Phase 1 | If the answer is no |
|---|---|---|---|
| **DEC-001** | **Confirm PACK_ROOT.** Is the observed path still the authoritative pack location for this program? | Every integrity re-check and every sibling path depends on it | Phase 1 waits; nothing is written beside a path nobody confirmed |
| **DEC-002** | **Supply UPGRADE_ROOT.** Where does `grok-intelligence-upgrade-v1` live? | BLOCK-001. Nothing in section 8 has a home until this is answered | No scaffolding is created, and the proposal stays a proposal |
| **DEC-003** | **APPROVE PHASE 1, or not.** Approval also confirms the writer and gate: docs writer in GitHub, COO first QC, PA last gate, Grok seats scope and QC only | Phase 1 does not begin without it | Phase 0 stands as a review artifact and nothing follows it |
| **DEC-004** | **The pilot.** Confirm `book-conceptual-editor` and the one narrow workflow in section 9, and confirm whether a capability exercise on owner-supplied material is exempt from that seat's do-not-write instruction (BLOCK-011) | The pilot cannot start without it, and the exemption question is not this report's to answer | No pilot runs; the recipe is not written |
| **DEC-005** | **May Phase 1 scaffolding be created as a sibling directory after approval?** | Creating files is a separate permission from approving the plan | Phase 1 stays a plan on paper |
| **DEC-006** | **CSO, CCO, and Pendulum: define them, or keep them gated for Phase 1?** | BLOCK-002. Undefined, they cannot appear in any map, KB row, or routing rule without inventing a meaning | They stay gated and are excluded from Phase 1 scope |
| **DEC-007** | **Pilot inputs.** Will KB-AUTHOR and KB-EDITORIAL content and an evaluation excerpt be supplied, or does the pilot wait? | Both knowledge bases are MISSING as pack content and as repo content, and no manuscript exists. Nothing is invented to fill them | The pilot waits, and the gap stays named |
| **DEC-008** | **Will a SHA-256 be recorded for `phase0-public-inventory.txt` and `phase0-qwen-draft.txt`?** Two digests for two files that already exist — no new run, no new access, nothing opened | BLOCK-019. Every Qwen-sourced finding in sections 4–7 is capped at SELF-REPORTED for want of them, including the strongest negative on the page | The inventory stays SELF-REPORTED and Phase 1 proceeds knowing its own evidence floor |

## 13. Next Authorized Action

Phase 0 is ready for independent review. No Phase 1 work, employee activation, routine creation, connector change, local mutation, or external action has been performed.

**COO is first QC. PA last-gates.** Run [reviews/last-gate-checklist.md](../../../reviews/last-gate-checklist.md) before anything leaves anyone's hands, and hand anything external to Michael. **Do not merge the pull request carrying this page until the PA last-gates it**, and do not restamp any last-gated leftover-seat plan to match it.

Source: the owner's Phase 0 brief and the operator's Qwen-sit follow-up; the sanitized 2026-08-25 office-Mac evidence session carried in [PR 141](https://github.com/platformology/company-os/pull/141); the `seats.json` extract `seats-summary.txt`; the 14:27:41–14:30:17 filename-only public inventory `phase0-public-inventory.txt` and `phase0-qwen-draft.txt`; [SOURCES.md](../../../SOURCES.md), [locks.md](../../locks.md), [company-facts.md](../../company-facts.md), [people.md](../../people.md), [offers.md](../../offers.md), [clients.md](../../clients.md), [how-money-moves.md](../../how-money-moves.md), [research-basis.md](../../research-basis.md), [runtime-openclaw.md](../../runtime-openclaw.md), [runtime-wiring.md](../../runtime-wiring.md), [seat-job-map.md](../../seat-job-map.md), [leftovers/README.md](../README.md), [leftover-write.md](../../leftover-write.md), [reviews/last-gate-checklist.md](../../../reviews/last-gate-checklist.md)
