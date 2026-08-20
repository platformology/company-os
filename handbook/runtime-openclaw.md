# Runtime — OpenClaw, the runtime we did not have to build

Recorded 20 Aug 2026 — Michael: **OpenClaw is the pile that already exists** for building real seat-workers. This page is that pile read against our twenty-three seats — what it already does, which parts of it we take, which parts we refuse, and how a person would know a seat is a worker instead of a page.

**Nothing here installs anything.** OpenClaw is not on this Mac, this page does not put it there, and no step below runs a command. This repo is markdown ([README.md](../README.md)); reading this page is the whole job today.

Where it sits: [runtime.md](runtime.md) is the build map for the four pieces — brain, hands, wiring, guts. This is a page beside those four, not a fifth piece. It names the outside runtime the four are already shaped like, so nobody sets out to design something a public project already finished.

What came after it: [engine.md](engine.md) takes the reading below and writes the files the shape expects — one workspace folder per seat, the five bootstrap files inside each, and an honest per-seat read of the public skill registry. That page is a draft on its own branch and it installs nothing either.

## What OpenClaw already is

[openclaw/openclaw](https://github.com/openclaw/openclaw) is a public MIT-licensed personal-assistant runtime, developed in the open by the OpenClaw Foundation, built for one operator running it on their own machine. Four parts of it matter here, and every one of them is something we would otherwise be inventing:

- **A gateway.** One local control plane that holds sessions, tools, events, and channel connections. Everything else — the CLI, the web UI — talks to it.
- **An agent workspace.** Each agent gets one directory that is its home and its working directory. The docs' own phrasing: keep it private and treat it as memory.
- **Bootstrap files that get injected.** Inside that workspace OpenClaw expects a small fixed set of plain markdown files, and on the first turn of a session it puts their contents into the prompt: `AGENTS.md` (operating instructions), `SOUL.md` (persona, boundaries, tone), `IDENTITY.md` (name and vibe), `USER.md` (who it works for), `BOOTSTRAP.md` (a one-time first-run ritual, deleted once it's done), `MEMORY.md` (long-term memory, only when it exists). A blank file is skipped. A **missing** file gets a "missing file" marker in the prompt rather than being quietly filled in.
- **Skills, loaded off disk.** A skill is a folder with a `SKILL.md` in it — YAML frontmatter carrying a `name` and a one-line `description`, then plain markdown telling the agent how and when to do the job. They load from a fixed precedence list, workspace first, then project, personal, managed, bundled, and extra directories, and the list is snapshotted when a session starts.
- **Multi-agent.** Several isolated agents in one gateway, each with its own workspace, its own state directory, its own session store, its own skill allowlist, and its own tool allow/deny list. Inbound messages reach the right agent through explicit bindings.

None of that is ours to design. It exists, it's documented, and people run it every day.

## Our twenty-three seats on that shape

| What OpenClaw calls it | What we already call it | Where ours lives |
|---|---|---|
| An agent | A seat | [seats/](seats/README.md) — one page per seat, the source of truth for what it owns |
| The agent workspace, `SOUL.md` + `AGENTS.md` | The body | [bodies/](bodies/README.md) — one runnable file per seat, complete inside itself |
| `BOOTSTRAP.md`, the first-run ritual | The desk you sit down at | [desks/](desks/README.md) — pages to open, first wake, what done looks like |
| A skills folder | Our skills folder | [skills/](../skills/README.md) — one folder per job, `SKILL.md` with the same `name` + `description` frontmatter |
| Per-agent skill allowlist | The seat's router row | [seat-job-map.md](seat-job-map.md) — one skill per seat, named, not chosen at runtime |
| Per-agent tool allow/deny | The seat's hands | [runtime-body.md](runtime-body.md) — the tools in the row are the whole set, and what's denied is written down |
| The model behind an agent | The shared office hand | `office-hand` = `qwen3.8:27b-q8_0` on this M1, Michael's word 20 Aug 2026 — see [bodies/README.md](bodies/README.md) |
| Bindings and routing | The wire | [runtime-wiring.md](runtime-wiring.md) — each seat's own Grok Bot chat, no bus installed |
| Whoever owns and checks the work | Grok Bot | Grok Bot stays the manager ([desks/BUILD.md](desks/BUILD.md)); the three QC layers are on [runtime-wiring.md](runtime-wiring.md) |
| Whoever writes the operating files | Claude, in GitHub | [runtime.md](runtime.md): Claude / Other Models writes the heavy pages, seats QC, and the PA is not the workhorse |

Two things that table is too narrow to hold:

**One hand, twenty-three bodies.** OpenClaw lets every agent point at its own model, and we do not use that. Ours all point at the same local weights, and the local-model path in OpenClaw is the same shape ours already is — one Ollama server on the machine, models addressed as `ollama/<model>`, several agents sharing it. **Seats are never rebuilt as local models** ([locks.md](locks.md)); what changes per seat is the body text, never the weights.

**Separate workspaces are the point.** OpenClaw is blunt that two agents must never share a state directory, because their auth and sessions collide. Our version of that rule is older and simpler: one page per seat, and where a body and a seat page disagree, the seat page wins.

## What we copy

Four things, and why each one earns its place.

1. **Skill-load.** A job is a folder with a `SKILL.md` in it, found on disk, named by its frontmatter rather than by where somebody filed it. We already write skills that way, so this is confirmation, not a change — and it settles the argument about whether a skill is a folder or a paragraph in a bigger page. It is a folder.
2. **Workspace files.** A seat's operating text lives in a few small named files that get read at the start of every session, not in one wiki page somebody has to remember to open. Ours are the body and the desk. Copy the split too: OpenClaw keeps voice in `SOUL.md` and operating rules in `AGENTS.md`, which is why a body carries tone and a router carries steps.
3. **Allowlists.** What a seat may touch is a written list, and a list that is set is the *whole* list — OpenClaw's per-agent skill list replaces the default rather than adding to it. That is [runtime-body.md](runtime-body.md)'s rule in someone else's words: the tools in the row are not preferred tools, they are all of them. Their own caveat travels with it — an allowlist is a list, not a guard; it does not stop a hand that was never listed, so the written denial still has to be read and obeyed.
4. **The sit-down loop.** Session starts, the files get read, the skill list is fixed for that session, the work runs, and a change to the files takes effect on the *next* session rather than mid-pass. That is our pass exactly: open the desk, open the router, run one unit, last-gate, stop ([cheap-loop.md](cheap-loop.md)).

One smaller habit worth stealing outright: when a file is missing, OpenClaw injects a marker saying so instead of skipping quietly. That is **named missing stays named missing**, enforced by a runtime. Ours is enforced by whoever is reading, which is weaker, so read like it matters.

## What we do not copy

**The lock, plainly: no send without Michael — nothing goes to a client, a prospect, or the public without his sign-off ([locks.md](locks.md)).**

Most of what makes OpenClaw fun is a mouth. It joins WhatsApp, Telegram, Slack, Discord, Signal, iMessage and more, streams replies into them as it thinks, pairs unknown senders, and can pass messages agent to agent. Every one of those is a way for text to leave the building without Michael reading it first, and an allowlist of approved senders does not fix that — it decides who may talk to the seat, not who the seat may answer. So:

- **No channels.** No channel bindings, no pairing, no sender allowlists, no group chats. The seats' own Grok Bot chats stay the whole wire ([runtime-wiring.md](runtime-wiring.md)), and they are read by us, not by the public.
- **No agent-to-agent messaging as a feature.** A handoff is a report messaging its owner's chat, and it waits in that chat until the owner's next window. That wait is the design.
- **No scheduled wakes beyond the ones we have.** Weekday 8am, then 11, 2, and 5. No hourly wakes, no heartbeat, no cron.
- **No skill registry installs.** OpenClaw can pull community skills off a public registry; ours are written here, credited in [SOURCES.md](../SOURCES.md), and reviewed by a person. Their own security note says treat third-party skills as untrusted code — we agree, and we go one further by not fetching them.
- **No sandboxes, containers, or VMs to make any of it work.** No VMs, no GKE ([locks.md](locks.md)).
- **No per-seat model.** See above; one hand, twenty-three bodies.
- **No install.** Not off this page, not as a side effect of reading it.

## Done-check — a worker, not a markdown body

A seat is a **worker** when a person can watch it do these, in order, without the PA writing any of it:

1. **It has a body and a desk on disk**, same slug as its seat page — [bodies/](bodies/README.md), [desks/](desks/README.md).
2. **Its router is a real folder** in [skills/](../skills/README.md), the one named in its row on [seat-job-map.md](seat-job-map.md), and it opens that folder itself.
3. **It touches only the hands in its row** on [runtime-body.md](runtime-body.md), and it can say out loud which ones those are and what it's denied.
4. **It takes the next named leftover** for its own job and finishes it, or says the queue is honestly empty and names where it looked ([runtime-guts.md](runtime-guts.md)).
5. **It hands the finished thing to its owner's chat** and stops — the PA did not carry it ([runtime-wiring.md](runtime-wiring.md)).
6. **Nothing was sent.** The draft exists and stops with Michael.

Six for six is a worker. A body file with nobody running it is a page — a good one, but a page. The check that this repo genuinely cannot make is whether any of it is actually wired up on the Mac; that one gets confirmed at the machine, on [desks/BUILD.md](desks/BUILD.md).

### Still named missing on this Mac

Honest list, because the page above would otherwise read as if we are further along than we are:

- **The OpenClaw gateway is not installed on this M1.** Not partly, not in a folder somewhere — it is not here. Everything above is a shape we recognise, not software we run.
- **The office hand has no Notion and no Gmail.** The five connected tools — Notion, Gmail, Calendar, Slack, Google Drive — are hands the Grok seat has. A body run in the local Qwen hand has no files and no browser, and it cannot open a Notion page ([bodies/README.md](bodies/README.md)). That gap is exactly what a gateway would close, and it is not closed.
- **HubSpot is out.** Closed, and not a system of record ([clients.md](clients.md)).
- **Bench is out.** No connector, so no ledger figure comes off this Mac ([runtime-body.md](runtime-body.md)).
- **Slack is connected and no seat's job sources it.** Michael names the job that uses it, or it stays unused.
- **The lock pages and the hand pages still disagree.** [locks.md](locks.md) and [runtime-brain.md](runtime-brain.md) read "no local LLM until Michael says go"; [bodies/README.md](bodies/README.md) and [desks/BUILD.md](desks/BUILD.md) name `office-hand` as already on the machine. That is Michael's to settle, it is already flagged as a leftover on both of those pages, and until he settles it the lock page governs. This page does not settle it either.

## Leftovers

- Michael says whether OpenClaw is ever installed here. Until he does, this page is a read, not a plan, and nobody opens the question by installing it to see.
- If it is ever installed, the first thing to check is what the office hand can reach — the Notion and Gmail gap above is the reason anyone would want a gateway at all.

## What we reused

Searched public GitHub first, per [reuse-what-github-has](../skills/reuse-what-github-has/SKILL.md). Everything named below is public and none of it is a Platformology program repo:

- [openclaw/openclaw](https://github.com/openclaw/openclaw), `README.md` — the gateway as one local control plane for sessions, tools, events, and channels, and the split between the runtime and the channels bolted onto it. Its installer, its channel list, and its companion apps were left behind.
- [docs.openclaw.ai/concepts/agent](https://docs.openclaw.ai/concepts/agent) — one workspace per agent, the injected bootstrap files, the "missing file" marker in place of a quiet skip, and skills loaded from a precedence list. Its sandbox, session, steering, and streaming machinery was left behind.
- [docs.openclaw.ai/concepts/agent-workspace](https://docs.openclaw.ai/concepts/agent-workspace) — the workspace file map, treat-it-as-memory framing, and the `AGENTS.md`-for-rules / `SOUL.md`-for-voice split that our desks and bodies already use.
- [docs.openclaw.ai/tools/skills](https://docs.openclaw.ai/tools/skills) — the loading order, the per-agent allowlist that replaces rather than merges, the note that an allowlist is not an authorization boundary, and the session snapshot that makes a skill change land on the next pass.
- [docs.openclaw.ai/tools/creating-skills](https://docs.openclaw.ai/tools/creating-skills) — a skill is a directory with a `SKILL.md`, `name` and `description` required, folder path for filing only. Its publishing flow and proposal queue were left behind.
- [docs.openclaw.ai/concepts/multi-agent](https://docs.openclaw.ai/concepts/multi-agent) — several isolated agents in one process, never sharing a state directory, with per-agent tool allow/deny. Its bindings, channel accounts, and agent-to-agent messaging were read and deliberately **not** adapted: they are the send path this repo locks.
- [docs.openclaw.ai/concepts/soul](https://docs.openclaw.ai/concepts/soul) — voice in one short file, operating rules kept out of it.
- [docs.openclaw.ai/concepts/model-providers](https://docs.openclaw.ai/concepts/model-providers) — the local Ollama provider, one server on the machine addressed as `ollama/<model>`, which is the same one-hand-many-bodies shape [bodies/README.md](bodies/README.md) already records.

The row for the repo is in [SOURCES.md](../SOURCES.md). No client, price, person, KPI, or machine fact came from any of it — the facts on this page are Michael's word or already recorded in this handbook.
