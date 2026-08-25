# Workforce pack deployment report — evidence packet

**Written: 25 Aug 2026.** **Evidence session: 2026-08-25, America/Denver.** **Status: not last-gated.**

Michael asked for a final Grok Bot → OpenClaw workforce installation evidence packet. This is that packet, written honestly.

**Installation and activation were not performed.** No pack skill was installed. No employee was activated. No acceptance run was executed. What was performed on the office Mac is a read-only preflight plus the pack's own offline test scripts. Everything below is labeled by what the supplied evidence actually carries.

Platformology LLC is the legal entity. **Promote a Book** and **Book Retreat** are DBAs of it — not two companies, and not SmarterVoice ([company-facts.md](../../company-facts.md)). **COO is first QC. PA last-gates.** **KPI "Current" stays empty** — no figure, including 0. No client, money, person, holder, or pipeline is created by this packet. Named missing stays named ([SOURCES.md](../../../SOURCES.md)).

## The four files in this packet

| File | What it is |
|---|---|
| `DEPLOYMENT_REPORT.md` | This page — what is proven, what is not, and what failed |
| [`seat-results.csv`](seat-results.csv) | 46 seats, one row each, plus header |
| [`acceptance-results.json`](acceptance-results.json) | Zero runs, stated as zero |
| [`sanitized-evidence.txt`](sanitized-evidence.txt) | Evidence file inventory and hashes |

## Label key — read this before any row below

| Label | What it means here |
|---|---|
| **PROVEN (hash-anchored)** | An evidence artifact exists, its SHA-256 was supplied, and a command, timestamp, and exit code were supplied |
| **PROVEN (console record)** | Command, timestamp, and exit code were supplied, but **no evidence filename or SHA-256 was supplied**. The artifact hash is UNVERIFIED. This is not hash-anchored proof and must not be cited as one |
| **SELF-REPORTED** | An operator said it. No independent artifact, scan, or hash exists. Do not upgrade to PROVEN |
| **UNVERIFIED** | Not measured, not run, or the number/hash/timestamp/exit code was not supplied |
| **FAILED** | A check ran and did not pass, or a stated requirement is not met |

**Absence of evidence is never PASS.** No SHA-256, exit code, timestamp, agent ID, fixture ID, or test score appears in this packet unless it was supplied. Where a value was not supplied it is written as UNVERIFIED rather than guessed.

## Machine

| | |
|---|---|
| Machine | Office Mac, hostname in evidence `MacBookPro`, America/Denver |
| OS (from OpenClaw status) | macos 26.6.2 arm64, node 24.15.0 |
| Evidence directory | `/Users/mdrew/Company/Jobs/workforce-pack-evidence-2026-08-25` |
| Pack root | `/Users/mdrew/Documents/Codex/2026-06-29/you-are-in-coding-execution-mode/grokbot-openclaw-workforce-pack` |
| ZIP under test | `.../grokbot-openclaw-workforce-pack-2026-08-25.zip` |
| OpenClaw CLI | `/Users/mdrew/Company/Engine/bin/openclaw` — **not on the default PATH** |

One machine, one operator. No second machine is in scope and none is named here.

## A. Package integrity — PROVEN (hash-anchored)

Two hash comparisons and five offline pack tests. All exit 0.

| # | Claim | Command | Timestamp (MDT) | Exit | Evidence file | Evidence SHA-256 | Label |
|---|---|---|---|---|---|---|---|
| A1 | ZIP SHA-256 observed matches expected: `d39a2cafacd6b44b7bd976871c7eac6271aa0ef696fc5382f57c3769b2f71975` | `shasum -a 256` on the ZIP | 2026-08-25 14:07:44 | 0 | `01-zip-sha256.txt` | `4266f5b41066e337053b74144f3675a80a44c1d14841d1d3b4f3ddd94338c2f9` | **PROVEN (hash-anchored)** |
| A2 | `SHA256SUMS.txt` SHA-256 observed matches expected: `7d02915d72134d2fa7175b6ab920f25d251b0d336af5d0664afce4d49f475cfc` | `shasum -a 256` on `SHA256SUMS.txt` | 2026-08-25 14:07:44 (same session) | 0 | `02-sha256sums-txt-sha256.txt` | `7ab60de4bad21573a4412486cbb9199699e1cfeab9c35b70f7c8ff51b8fcc4d1` | **PROVEN (hash-anchored)** |
| A3 | 91 file checksums verified | `node scripts/verify_checksums.mjs` | 2026-08-25 14:07:53–14:08:56 window | 0 | `03-verify-checksums.txt` | `6c0ccb76c4cd0a29821a9f2cca07f881167a30e43b765b1c2e280cfee413154f` | **PROVEN (hash-anchored)** |
| A4 | 46 unique seats; status and holder invariants preserved; 47 text-only skills validated; 23 craft acceptance fixtures and 92 role-qualified traps validated | `python3 -S scripts/validate_pack.py` | 2026-08-25 14:07:53–14:08:56 window | 0 | `04-validate-pack.txt` | `2c5e909650b8970d80b419fd09882026de5fa1b0174a6438573a5dc76292c1df` | **PROVEN (hash-anchored)** |
| A5 | Candidate bundle contains only selected skills, tool policy, allowed fixture inputs, task metadata and checksums | `python3 -S scripts/test_materialize_candidate_bundle.py` | 2026-08-25 14:07:53–14:08:56 window | 0 | `05-test-materialize-candidate-bundle.txt` | `3a1dbcde2a7d4453b2aa33fa785ea39a4a009b96c2cf89e4dae130c1e19ad81d` | **PROVEN (hash-anchored)** |
| A6 | Planner accepts a confirmed one-to-one map and blocks duplicate, unknown, and empty targets | `python3 scripts/test_plan.py` | 2026-08-25 14:07:53–14:08:56 window | 0 | `06-test-plan.txt` | `b3cb7c55e0670a7a3fe6c81880e5b584a3e8a3226ef704648d95ebe7822cfa24` | **PROVEN (hash-anchored)** |
| A7 | 47 exact local skill hashes allowed; plugin, future, network and unknown targets blocked | `node scripts/test_install_policy.mjs` | 2026-08-25 14:07:53–14:08:56 window | 0 | `07-test-install-policy.txt` | `60d929c73414299cf33ad492d70b6d76523f5f39c5bcb5a00ba513d52f929aad` | **PROVEN (hash-anchored)** |

A3–A7 ran from the pack root. The supplied timestamp is the **window** `2026-08-25 14:07:53–14:08:56 MDT` covering all five; the per-script start time inside that window is **UNVERIFIED**.

**What A does not prove.** A validated package is not an installed package. The 47 skills in A4 and the 47 allowed hashes in A7 are the pack's own inventory and policy, checked offline. **Nothing in A shows a skill placed on an agent, and A7 is an allow-check, not an install.**

## B. Grok Bot — SELF-REPORTED

| Claim | Label | Basis |
|---|---|---|
| This pack session created 0 Bots, changed 0 Bots, deleted 0 Bots | **SELF-REPORTED** | Operator statement. No exported bot audit, log, or hash was supplied |
| No pack skills imported into Grok Bot | **SELF-REPORTED** | Operator statement |
| No candidate bundles uploaded | **SELF-REPORTED** | Operator statement |
| `craft-acceptance.v1.json` and evaluator-only fields were not placed in Grok chat, memory, attachments, or shared workspace | **SELF-REPORTED by the COO operator** | **No independent forensic scan was run.** Do not upgrade this to PROVEN. The absence of a scan is not a clean scan |
| 23 Grok Bot chats already exist for assigned / leftover / parked seats | **SELF-REPORTED** | Read off the Grok Bot teammate list. **Not created by this pack** |
| The 23 craft seats have no Grok chat | **SELF-REPORTED** | Same teammate list |
| No disposable bench tests were run; cleanup none required | **SELF-REPORTED** | Operator statement. No bench test artifact exists to clean up |
| Tools, browser, terminal, approvals, and routines used for pack install: none | **SELF-REPORTED** | Consistent with no install having happened |
| Grok clocks remain paused | **SELF-REPORTED** | Operator statement. No clock-state export was supplied |

**The 23 pre-existing Grok Bot chat IDs.** These are recorded because they already existed. **No other ID is to be written anywhere in this packet.**

| Seat | Existing Grok Bot chat ID |
|---|---|
| pa | `b2978a95-b098-4d50-864b-6fa2bf7477ff` |
| coo | `e6d4d12a-6c80-4d85-8140-17ab73a54a64` |
| cto | `2a4abb44-fadc-4103-91d6-3735e434872c` |
| cfo | `f06124d7-9cf8-4f2a-844f-b4265c64816e` |
| cmo | `83f762c1-bf71-427d-8be1-6b7660dbb42d` |
| cso | `8f3baca0-a9f0-49c9-a8c0-18461185d507` |
| cco | `2f8279cd-e73b-4457-b5d6-2cb7f73553a4` |
| chro | `88ecf9ee-9f63-412c-9b31-4e2d7f977f9f` |
| controller | `e61899af-2471-4eb5-9675-e14627ad11a3` |
| bookkeeper | `750215eb-efa1-4f74-888a-4e944f963da5` |
| people-ops | `0d3c8de9-083d-4b45-b039-8cab045c6111` |
| head-of-content | `437dcc32-1b39-411e-91be-1059938588cf` |
| head-of-author-success | `dd4aafeb-2511-4d4d-b0c3-b970228c3785` |
| client-success | `0b393c69-cdb0-4768-ac3b-d6b8a3fb348d` |
| vp-campaigns | `601b33e7-5326-46c3-911c-ac001c843e2f` |
| campaign-coordinator | `9e30c691-15b3-483e-9c28-ce6f21f9c025` |
| vp-retreats | `ec1781d5-71bb-47f2-8b4c-3225d507a810` |
| retreat-producer | `ad2d9470-8b70-495b-bd0a-a79bb0453664` |
| head-of-demand | `94f1b097-37cb-41fb-b7c8-83e6fc8d6fe6` |
| head-of-sales | `e4bf6802-6708-4b97-ab3b-ded2a6a5577c` |
| sdr | `6d649a32-8ace-4d81-b87b-5a062de1283c` |
| head-of-engineering | `e6646393-5ad9-4379-8aee-851e7aafafcd` |
| developer | `a3d1d5d2-f21e-442e-b27e-acec16b8e08f` |

## C. OpenClaw — mixed, with one FAILED boundary

| # | Claim | Command | Timestamp (MDT) | Exit | Evidence file | Evidence SHA-256 | Label |
|---|---|---|---|---|---|---|---|
| C1 | OpenClaw 2026.7.1-2 (0790d9f) | `/Users/mdrew/Company/Engine/bin/openclaw --version` | 2026-08-25 14:09:23 | 0 | not supplied | UNVERIFIED | **PROVEN (console record)** |
| C2 | `Config valid: ~/.openclaw/openclaw.json` | `openclaw config validate` | not supplied — UNVERIFIED | 0 | not supplied | UNVERIFIED | **PROVEN (console record)** |
| C3 | 46 existing agent IDs matching the 46 seat slugs; default `cto`; model on all listed `ollama/office-hand`; bindings 0 | `openclaw agents list --json` | not supplied — UNVERIFIED | 0 | not supplied | UNVERIFIED | **PROVEN (console record)** |
| C4 | Security audit: critical 0, warn 1, info 1 | `openclaw security audit --json` | 2026-08-25 14:09:36 | 0 | `openclaw-security-audit.json` | `93a9617be803cdcdbfff3eeb09e08ace11a766aa54823cd0b76d8bc0f9f19fc7` | **PROVEN (hash-anchored)** |
| C5 | Official `preflight.sh` passes when `Engine/bin` is on PATH | `preflight.sh` with PATH including `Engine/bin` | 2026-08-25 14:10:04 | 0 | `preflight.txt` | `8e68ea39888e3d8316c6100cd67378b432b18599cfcc7cccfe9f2b28bb05f5b4` | **PROVEN (hash-anchored)** |
| C6 | MCP servers: `[]` | not supplied — UNVERIFIED | not supplied — UNVERIFIED | not supplied — UNVERIFIED | `openclaw-mcp.json` | `bb5f31e329c66c21d51fe0bce9b33ef704cf487c9decafaeda07ef1831382a37` | **PROVEN (hash-anchored artifact; command, timestamp, exit code UNVERIFIED)** |
| C7 | 32 bundled plugins, all enabled and loaded | not supplied — UNVERIFIED | not supplied — UNVERIFIED | not supplied — UNVERIFIED | `openclaw-plugins.json` | `76dab26c7dd7816ece9e2428f047a52ac193c2741389f774cbd218ada53c7a00` | **PROVEN (hash-anchored artifact; command, timestamp, exit code UNVERIFIED)** |
| C8 | 63 skills in inventory across sources `openclaw-bundled` / `extra` / `workspace` / `agents-skills-personal` | not supplied — UNVERIFIED | not supplied — UNVERIFIED | not supplied — UNVERIFIED | `openclaw-skills.json` | `bc38f94972621dce83c8be450577870cdea8ad8235ab806da42cef017b0764cb` | **PROVEN (hash-anchored artifact; command, timestamp, exit code UNVERIFIED)** |
| C9 | Gateway local loopback `ws://127.0.0.1:18789` reachable; LaunchAgent loaded and running; Tailscale off; Agents 46; 46 bootstrap files present; sessions 37; default `cto` | `openclaw status --usage` | not supplied — UNVERIFIED | not supplied — UNVERIFIED | `openclaw-status-usage.txt` | `f531633fb4f9426272e2060028cabfd87a35cb6892685feb2a0950d74e4f404c` | **PROVEN (hash-anchored artifact; command timestamp and exit code UNVERIFIED)** |

**The 46 OpenClaw agents already existed. This pack did not create them.** An agent existing is not an employee activated and not a seat staffed.

### C4 audit detail, as supplied

- **Warning — `gateway.trusted_proxies_missing`**: loopback bind, `trustedProxies` empty.
- **Info**: `tools.elevated` enabled; `hooks.webhooks` disabled; `hooks.internal` disabled; browser control enabled; trust model "personal assistant, one operator"; groups open 0, allowlist 0.

### C10 — Gateway and OS-user separation: **FAILED**

Separation of finance, people, legal, and production as **independent boundaries** is **FAILED**. There is one gateway, one OS user, and 46 agents sharing both. That is **PROVEN** by the `agents list` result (C3) plus the audit's own trust model (C4, hash-anchored). **No separate OS users exist and none are invented here.** `tools.elevated` and browser control being enabled on that shared gateway is on the deviation list below.

### C11 — Pack skills on agents: **UNVERIFIED / not installed**

- The pack's **47 workforce skills were NOT installed this session.**
- **Per-agent pack skill hash verification: UNVERIFIED** — it was not run. Not "clean," not "no findings." Not run.
- The 63-skill inventory (C8) includes `clawhub` as eligible. **It was not installed and is not to be installed here.**
- The 32 bundled plugins (C7) are **inherited and stay enabled.** This leftover does not disable them.

## D. Ollama and hardware — partly recorded, key numbers UNVERIFIED

Recorded 2026-08-25 14:07:55 MDT. **No exit code was supplied for any command in this section, so every exit code here is UNVERIFIED.**

| Claim | Label | Note |
|---|---|---|
| `ollama version` 0.32.14 | **PROVEN (console record)** — exit code UNVERIFIED | Timestamp 2026-08-25 14:07:55 MDT |
| `qwen3.8:27b-q8_0` exists, id `8f5fb6b71ea0`, size 29 GB | **PROVEN (console record)** — exit code UNVERIFIED | |
| `show`: architecture qwen35, parameters 27.3B, context length 262144, quantization Q8_0 | **PROVEN (console record)** — exit code UNVERIFIED | Model-declared maximum context, not the configured context |
| `ollama ps` during this check: `coo:latest`, id `9dc7ca0ed707`, size 29 GB, processor 100% GPU, context 8192, until 24 hours from now | **PROVEN (console record)** — exit code UNVERIFIED | **This was not a pack acceptance workload.** It proves a process was resident, nothing about pack performance |
| Listener `127.0.0.1:11434` | **PROVEN (console record)** via `lsof` — exit code UNVERIFIED | Loopback only |
| `OLLAMA_HOST` and `OLLAMA_NO_CLOUD` are empty | **PROVEN (console record)** via `launchctl getenv` — exit code UNVERIFIED | Unset, not set-to-empty-on-purpose as far as the evidence shows |
| Configured observed context this sit: 8192 | **PROVEN (console record)** — exit code UNVERIFIED | |
| Safe pack start 32K applied | **FAILED — not applied** | The recommended safe start was not in place during this sit |
| 64K tested | **UNVERIFIED — not tested** | |
| Peak memory, swap, latency, tokens/sec under a representative pack workload | **UNVERIFIED** | **No pack workload was run.** There is nothing to report and nothing is estimated |

**Evidence hashes for this section**, labels `09a`–`09e`. The **mapping from each label to its command and full filename was not supplied**, so the mapping is UNVERIFIED and is not guessed:

- `09a` `3f4c567c941c46b6b3af35d7e9b56ef75561416fe7a60406d6966cd63b8e65f1`
- `09b` `372dbd9f3cd0c582cf0a7f411cda83f879ec76084e2b9c575e871fca8c0e2b6c`
- `09c` `2100b92c2c0cdfe8aee6398f951f64cfb9f3db705aaa46e9474d4f9bde99b0d1`
- `09d` `da2c9c940fe9ddf4c10de5f48c976d019afb0ffa0bcaea842b44821918e27ee0`
- `09e` `fb47de6111cb3c65a448e88a49dc60fb0c626582f24d87e311b25eb11c2410f7`

No token, key, or credential is reproduced anywhere in this packet.

## E. Acceptance tests — zero runs

**Zero acceptance runs were executed.** Therefore:

- **No role has three clean final-configuration runs.**
- **No role is activation-ready.** All 46 seats read `NOT_ACTIVATION_READY` in [`seat-results.csv`](seat-results.csv).
- **Grok graded nothing.** No score, no pass, no fail.
- No fixture ID, score, or output hash appears in [`acceptance-results.json`](acceptance-results.json), because none was produced.
- **The hidden evaluator oracle is not in this packet** and is not to be added to it.

`acceptance-results.json` is an empty `runs` array plus the statement that 0 runs were executed. An empty array is the honest result. It is not a pass.

## F. Organization controls

**A skill built is not a bot activated.** Keep those two apart or this packet becomes a lie by summary:

| | Count | Label |
|---|---|---|
| Pack skills validated offline | 47 | **PROVEN (hash-anchored)** — A4 and A7 |
| Pack skills installed on an agent | 0 | **PROVEN by absence of any install action** — C11 |
| Permanent bots activated by this pack | 0 | **SELF-REPORTED** — B |
| Roles with 3 clean acceptance runs | 0 | **PROVEN by E** — zero runs executed |

### Expected disposition

The `expected_disposition` column in [`seat-results.csv`](seat-results.csv) is copied from the `ORG_DESIGN_AUDIT.md` recommendations for all 46 seats. It is **a recommendation, not a decision, and not an activation.** Nothing in this packet merges, retires, renames, or repurposes a seat.

### Roster status — PROVEN extract

Extracted from `seats.json`. Evidence `seats-summary.txt`, SHA-256 `73bc38eb86de888dce52765b90e52484eddaadc9897c20c79c654b3490e28a8e`, timestamp `2026-08-25T14:09:36-06:00`.

- **Only one holder is recorded: COO — Anthony C. Garcia.** Every other seat's holder is **not recorded**, and this packet does not name one.
- **`leftover_only`**: `head-of-demand`, `head-of-sales`, `sdr`. These three have **no live job**.
- **`parked`**: `head-of-engineering`, `developer`.
- **23 craft seats unassigned.**
- Those five seats stayed inactive as live jobs this session. OpenClaw agent IDs already exist for them — that is a pre-existing leftover-file person, **not a this-pack activation**, and it does not unpark anything or create a live job.

### Unresolved blockers — do not invent answers

- **CSO meaning** — unresolved.
- **CCO meaning** — unresolved.
- **Pendulum source hierarchy** — unresolved.
- **Who fills any seat besides COO** — not recorded.
- **Knowledge-source gaps** — unresolved.
- **Integration / connector decisions** — unresolved.
- **Membership price** — named missing, and the rest of the named-missing list stays named ([SOURCES.md](../../../SOURCES.md)).

## G. Deviations from the intended deployment

1. **The first OpenClaw lookup used PATH only and wrongly concluded OpenClaw was missing.** That check is **FAILED** and was later recut using `/Users/mdrew/Company/Engine/bin/openclaw`.
2. **Pack skills were not installed.** No activation. No three-clean acceptance. The deployment's whole point did not happen.
3. **Official `preflight.sh` would fail without PATH.** With `Engine/bin` on PATH it passed (C5). The wrapper depends on a PATH that is not the default.
4. **32 bundled plugins are all enabled** (C7). Inherited state, not chosen by this pack, and not disabled here.
5. **The `clawhub` skill is eligible in the inventory** (C8) and was **not installed** this session.
6. **`tools.elevated` and browser control are enabled on the shared gateway** (C4) — on the same gateway all 46 agents share.
7. **`gateway.trusted_proxies_missing` warning** stands (C4): loopback bind, `trustedProxies` empty.
8. **`OLLAMA_HOST` and `OLLAMA_NO_CLOUD` are unset** (D).
9. **Observed context was 8192, not the safe pack start of 32K, and 64K was never tested** (D).
10. **Peak memory and tokens/sec are UNVERIFIED** because no pack workload ran (D).
11. **No OS-user separation** for finance, people, legal, or production — **FAILED** as an independent boundary (C10).
12. **No Grok candidate-bundle bench tests were run** (B).
13. **Evidence file `10-openclaw-absent.txt` is stale and wrong** after the recut in deviation 1. Its SHA-256 was not supplied, so its hash is **UNVERIFIED**. It contradicts C1–C9 and must not be read as a current finding.
14. **This handbook's recorded state and the supplied evidence disagree, and this packet does not settle it.** [runtime-openclaw.md](../../runtime-openclaw.md) records the OpenClaw gateway as not installed on this Mac and the shared hand as not installed, and [locks.md](../../locks.md) reads "No local LLM until Michael says go." The evidence above records an installed OpenClaw gateway with 46 agents and a resident Ollama model on the office Mac. **How those reconcile is not recorded anywhere and is not decided here.** It is Michael's, via the PA last gate. Nothing in this packet lifts a lock, and nothing in it edits those pages.

## What this packet is not

- Not an activation, and not a permission to activate.
- Not a pass. Nothing here converts an absent check into a green one.
- Not a holder list, a client list, a price, a pipeline, or a KPI figure.
- Not an install instruction. It does not tell anyone to install a skill, a plugin, `clawhub`, or a model.

## Gate

**COO is first QC. PA last-gates.** This packet is docs only and nothing in it sends. Run [reviews/last-gate-checklist.md](../../../reviews/last-gate-checklist.md) before anything leaves anyone's hands, and hand anything external to Michael.

**Do not merge the pull request carrying this packet until the PA last-gates it.** Do not restamp last-gated leftover-seat plans to match it.

Source: the supplied 2026-08-25 office-Mac evidence session listed in [`sanitized-evidence.txt`](sanitized-evidence.txt), `ORG_DESIGN_AUDIT.md` (pack), `seats.json` extract `seats-summary.txt`, [SOURCES.md](../../../SOURCES.md), [locks.md](../../locks.md), [company-facts.md](../../company-facts.md), [people.md](../../people.md), [leftovers/README.md](../README.md), [leftover-write.md](../../leftover-write.md)
