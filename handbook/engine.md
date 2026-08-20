# The engine — the twenty-three seats, written the way a runtime expects them

Recorded 20 Aug 2026 — Michael: **build the engine out of what already exists, then put our names on it.** This is the human run page for that. It is a draft on a branch, it is not merged, and **nothing on it installs anything.**

[runtime-openclaw.md](runtime-openclaw.md) already did the reading: it took [openclaw/openclaw](https://github.com/openclaw/openclaw) — a public MIT-licensed personal-assistant runtime, developed in the open by the OpenClaw Foundation — and held it up against our twenty-three seats, and the finding was that we had been describing its shape by hand for weeks. This page takes the one step after that. It writes the files that shape actually expects, one folder per seat, so that what exists here is **the thing itself** rather than a description of the thing. Whether it is ever used is a separate question, and it is Michael's.

No runtime got designed here. Every file layout, file name, and loading rule below is OpenClaw's, documented and public. What is ours is the twenty-three seats and the words in them, and those were already written in [seats/](seats/README.md), [bodies/](bodies/README.md), and [desks/](desks/README.md).

## What the engine is

Three parts. None of the three is new, and that is the point.

**1. The OpenClaw shape.** A gateway on one machine that holds sessions, tools, and events. One private working directory per agent, which the docs tell you to treat as memory. A small fixed set of plain markdown files inside that directory, read into the prompt at the start of every session — `AGENTS.md` for operating rules, `SOUL.md` for voice and boundaries, `IDENTITY.md` for the name, `USER.md` for who it works for, `BOOTSTRAP.md` for the one-time first sit-down. Skills as folders with a `SKILL.md` in them. Several agents in one gateway, each isolated, each with its own workspace and its own allow list.

**2. Our twenty-three seats.** Already written, already sourced, already in conflict-checked agreement with each other. The engine adds no seat, no job, no client, no price, and no person. Where any file below and a seat page disagree, **the seat page wins** — same rule as [desks/README.md](desks/README.md), and it does not get relaxed because a file is now shaped like a runtime expects.

**3. One shared hand — named, not installed.** The shared always-on office hand is **Gemma 4 26B 8-bit on this M1**, and it is there **after Michael says go**, not before. That is recorded 19 Aug 2026 via the CTO and restated 20 Aug; it is named the same way on [runtime.md](runtime.md), [runtime-brain.md](runtime-brain.md), [bodies/README.md](bodies/README.md), and [desks/BUILD.md](desks/BUILD.md), and those pages own the rest of the picture. Two lines travel beside it so nobody reaches for the wrong one: **Llama 3.3 70B 4-bit on this M1** is the on-purpose pen, **not a second seat brain**, and no seat is built on it; **Flash 2-bit** is the M5, SmarterVoice only, and the M5 is parked. **Status today: not installed** — **"No local LLM until Michael says go"** is the lock's own wording on [locks.md](locks.md), and Phase 4 of the go packet is the only thing that lifts it. Twenty-three names would cost one set of weights, because **seats are never rebuilt as local models** ([locks.md](locks.md)) — and that lock does not lift because the seats now have workspaces.

Bolt those three together and a seat stops being a page you read and becomes a thing that opens its own desk. That is the whole ambition. It is not a product, it is not a bus, and it is not a dashboard.

## What this page will not write down

**No build command, no run command, no model tag, no context size, no sampler setting.** Not on this page, not in any of the twenty-three workspace folders, not as an example. Those are not recorded in this repo — they belong to the go packet behind Phase 4 on [locks.md](locks.md), and they stay named missing in [SOURCES.md](../SOURCES.md) rather than being guessed here. A guessed tag is a wrong tag, and a run line written today is Phase 4 taken early, which is a broken lock rather than a head start. [runtime-openclaw.md](runtime-openclaw.md), [bodies/README.md](bodies/README.md), and [desks/BUILD.md](desks/BUILD.md) all refuse the same thing in their own words, and this page does not become the one place a command leaks in.

**No name of who would stand this up.** Writing the files is this repo's job; deciding whether anything is ever assembled on the M1, and by whom, is Michael's. This page does not hand the folder to a model, to a new hire, or to anyone else.

## What is in this folder

```
handbook/engine.md                          this page
handbook/engine/workspaces/<slug>/          23 folders, one per seat
    SOUL.md         voice and boundaries
    AGENTS.md       operating rules
    IDENTITY.md     the seat's name, and who fills it
    USER.md         who the seat works for
    BOOTSTRAP.md    the first sit-down, run once
handbook/engine/clawhub-list.md             what exists on the public registry, per seat
```

The slugs are the same twenty-three already on [desks/README.md](desks/README.md) — `pa`, `coo`, `cmo`, `head-of-content`, `head-of-demand`, `cso`, `head-of-sales`, `sdr`, `cfo`, `controller`, `bookkeeper`, `cto`, `head-of-engineering`, `developer`, `cco`, `head-of-author-success`, `client-success`, `chro`, `people-ops`, `vp-campaigns`, `campaign-coordinator`, `vp-retreats`, `retreat-producer`. Same slug as the seat page, the body, the desk, and — after go, if a seat model is ever built — the name it would be built under ([desks/BUILD.md](desks/BUILD.md)). One slug everywhere, no translation table.

**Five files, and no sixth.** Four things OpenClaw also knows about are deliberately absent from every folder:

- **No `MEMORY.md`.** A memory file is supposed to hold what a seat actually learned. We have not run a session, so there is nothing to put in one, and a memory file full of plausible remembered facts is the worst artifact in this entire repo — it reads like history and it is fiction. Named missing stays named missing. When a seat has really run and really learned something, a person writes it then — which is what a real one looks like: the memory files in [sententialpeet/boslab-workspace](https://github.com/sententialpeet/boslab-workspace), a live workspace someone left public, are dated to sessions that actually happened.
- **No `memory/` daily logs**, for the same reason.
- **No `BOOT.md`.** That is OpenClaw's startup checklist, and it fires on gateway restart. We have no wake we did not already write down ([runtime-wiring.md](runtime-wiring.md): weekday 8am, then 11, 2, and 5), so there is nothing for it to hold.
- **No config, no credentials, no `skills/` copies.** Config lives outside the workspace on the machine. Skills are already folders in [skills/](../skills/README.md); they get pointed at, not duplicated into twenty-three places.

## Where each file came from

Nothing below was composed fresh. Each file is one existing page re-cut along the line OpenClaw draws.

| File | What it carries | Cut from |
|---|---|---|
| `SOUL.md` | Who the seat is, what it owns, what is not its seat, what it never does, and the sentence it says when it has to stop | The body — [bodies/](bodies/README.md) |
| `AGENTS.md` | The pass in order, the only hands it has, what "done" looks like, who it hands to, what it must never do | The desk plus the seat's router row — [desks/](desks/README.md), [seat-job-map.md](seat-job-map.md) |
| `IDENTITY.md` | The seat's name, its slug, its status, and who fills it | The seat page — [seats/](seats/README.md), and [people.md](people.md) for the holder |
| `USER.md` | Michael Drew, Platformology LLC, America/Denver, and the standing directives every seat works under | [company-facts.md](company-facts.md), [locks.md](locks.md), [runtime-body.md](runtime-body.md) |
| `BOOTSTRAP.md` | Open the locks, then open the desk, in the desk's own order | The desk's "Open these pages, in this order" list |

The split between `SOUL.md` and `AGENTS.md` is OpenClaw's and it is a good one: voice in one file, rules in the other. It is also the split our bodies and desks already had, which is why this re-cut was mostly scissors and not writing.

**`USER.md` is the same file twenty-three times, and that is deliberate.** Every seat works for the same man under the same locks. OpenClaw's convention for that file is dated directives — each line says when it was recorded and whether it is still live — and it gets its own 4,000-character budget in the prompt, so it stays short on purpose. A directive is superseded by Michael, in writing, with a date. Not by a seat, and not by a good argument.

## The names on it

This engine is Platformology's, not a template with the serial number filed off.

- **Platformology LLC** is the legal entity. **Promote a Book** and **Book Retreat** are DBAs of it — one company with two names the public sees, not two companies, and not SmarterVoice ([company-facts.md](company-facts.md)).
- **Michael Drew** is who every one of the twenty-three works for. Nothing reaches a client, a prospect, or the public without his sign-off.
- **America/Denver** is the clock. The calendar hand is the one already connected: michael@profluent.com ([runtime-body.md](runtime-body.md)).
- **Anthony C. Garcia — COO / Chief Persona Architect — is the one recorded seat holder.** His `IDENTITY.md` says so. The other twenty-two say **"not recorded,"** and they keep saying it until Michael records someone. A workspace existing for a seat does not fill the seat.
- **HubSpot is closed** and is not a system of record ([clients.md](clients.md)). No workspace reaches for it.
- **Bench has no connector.** It is the general ledger and nothing on this Mac reads it, so no ledger figure comes out of the money seats unless a person opened Bench by hand and is named as having done it.
- **The five connected tools are the whole set** — Notion, Gmail, Google Calendar, Slack, Google Drive. No sixth gets added to make a workspace work. Slack is connected and no seat's job sources it; that stays a leftover for Michael, not a hole to fill with a channel.
- **No number went into these files that wasn't already recorded.** No client, no price, no KPI, no headcount, no forecast. The track record stays uncollapsed. KPI Current stays empty.

## What we copied

Four things, each because it is load-bearing and each because refusing it would mean building our own version of the same thing.

1. **One workspace per seat.** OpenClaw is blunt that two agents must never share a state directory — their auth and their sessions collide. Ours is twenty-three folders that never touch.
2. **A small fixed set of injected files.** The seat's operating text is a handful of named files read at the start of every session, not a wiki page someone has to remember to open.
3. **The missing-file marker.** When one of those files is absent, OpenClaw puts a "missing file" note in the prompt rather than skipping quietly. That is **named missing stays named missing**, enforced by software instead of by whoever is reading. It is the one habit here that is strictly better than ours.
4. **Bring-your-own bootstrap files.** OpenClaw will seed those files itself if you let it. We do not let it — the config switch for that is `agents.defaults.skipBootstrap`, and it exists precisely for people who write their own. Ours are written, reviewed, and in git. Nothing gets auto-filled on top of them.

## What we refused

**The lock, plainly: no send without Michael.** Nothing goes to a client, a prospect, or the public without his sign-off ([locks.md](locks.md)).

Most of what makes OpenClaw fun is a mouth, and a mouth is exactly what this company has locked. So:

- **No channels.** No WhatsApp, Telegram, Slack, Discord, Signal, or iMessage binding. No pairing, no sender allow lists, no group chats. The seats' own Grok Bot chats stay the whole wire ([runtime-wiring.md](runtime-wiring.md)).
- **No send, at all, from any workspace.** Every `SOUL.md` and every `AGENTS.md` in this folder says it in its own words. A draft is a finished deliverable; a sent message is a lock break.
- **No agent-to-agent messaging.** A handoff is a report messaging its owner's chat and then waiting for the owner's next window. That wait is the design.
- **No scheduled wakes beyond the four we have**, and no heartbeat and no cron.
- **No registry installs.** ClawHub is real, it is public, and [clawhub-list.md](engine/clawhub-list.md) says honestly what is on it per seat — because the next person should not have to re-run that search. Nothing on that list gets installed. Their own security note says treat third-party skills as untrusted code; we agree, and we go one further by not fetching them.
- **No VMs, no GKE, no containers, no sandboxes** to make any of this work ([locks.md](locks.md)).
- **No per-seat model.** One hand, twenty-three bodies.
- **No install off this page.** Not as a step, not as a side effect of reading it.

## If these files are ever stood up

**Nothing below is a step anyone takes today.** OpenClaw is not installed on this M1, whether it is ever installed here is Michael's call, and this page does not hand the folder to anyone to assemble. What follows describes the state these files expect, so the folder is legible to whoever reads it later. A description is not an instruction.

### Three things that are Michael's, not ours

1. **OpenClaw is not on this M1.** Not partly, not in a folder somewhere. Whether it is ever installed here is his call, and nobody opens that question by installing it to see ([runtime-openclaw.md](runtime-openclaw.md)).
2. **The local-model lock reads "no local LLM until Michael says go,"** and every hand page in this repo agrees with it. [locks.md](locks.md), [runtime-brain.md](runtime-brain.md), [runtime.md](runtime.md), [bodies/README.md](bodies/README.md), and [desks/BUILD.md](desks/BUILD.md) all name Gemma 4 26B 8-bit as the shared hand and all of them wait on the go. There is no open disagreement here for him to settle, and this page does not manufacture one.
3. **This branch is not merged.** Draft. Do not merge it to make anything below reachable.

Until all three are settled, the honest state is: the files exist, and nothing has been stood up. That is a finished answer, not a blocked one.

### What the files expect

Four properties, described rather than commanded, and nobody is assigned here to produce them.

1. **One workspace directory per seat, contents verbatim.** OpenClaw is blunt that two agents must never share a state directory — their auth and their sessions collide. Twenty-three folders, twenty-three directories, no sharing. Verbatim means verbatim: not a name, not a price, not a lock, not a "not recorded." A file that looks wrong is a note back to a person, never an edit in flight.
2. **Bootstrap seeding off.** OpenClaw will seed its own starter files if you let it, and the config switch that stops it exists precisely for people who wrote their own. Ours are written, reviewed, and in git.
3. **No seat model exists yet, and this page does not describe building one.** After go the shape is one model definition per seat, every one pointing at the same shared weights with that seat's body file as its SYSTEM text. That shape is written out once, on [bodies/README.md](bodies/README.md), and that page carries no command for it either.
4. **Nothing gets installed to make any of this true** — not OpenClaw, not a model, not a skill off a registry, not a channel.

### What a person reads, if a seat's workspace is ever in front of them

You do not need to have read this whole page. Pick your seat and start.

1. **Read [locks.md](locks.md).** All of it, on the page itself. A new hire who skips it is the failure mode this repo exists to prevent.
2. **Open your seat's `BOOTSTRAP.md`** and do what it says, in its order. It opens the locks, then the seat page, then the body, then the router, then the Notion pages — the desk's own list, nothing added.
3. **Delete `BOOTSTRAP.md` when it is done.** That is OpenClaw's rule for that file and it is a good one: a first sit-down that keeps happening is not a first sit-down. Everything else stays.
4. **Read your `SOUL.md` and your `AGENTS.md`.** Between them they are the whole job: who you are, what you may touch, and how a pass ends.
5. **Run one pass.** One unit of work, off the desk, out of the seat's own named queue. One, then the gate — not two ([cheap-loop.md](cheap-loop.md)).
6. **Run [reviews/last-gate-checklist.md](../reviews/last-gate-checklist.md)**, every line, honestly.
7. **Hand the finished thing to your owner's chat and stop.** The owner is on your `AGENTS.md`, and it is the same one already on [runtime-wiring.md](runtime-wiring.md). The PA is not a relay in the middle of it.
8. **Nothing was sent.** The draft exists and stops with Michael.

If your seat is **parked** (Head of Engineering, Developer) or **unassigned** (Head of Demand, Head of Sales, SDR), steps 5 through 7 look different on purpose: the pass is naming the lock or the unassigned status, saying where the ask goes, and stopping. Those workspaces refuse work in both `SOUL.md` and `AGENTS.md`. Standing one of them up does not unpark or staff anything.

## Done-check, one seat at a time

Say the seat out loud, then check. This is [desks/BUILD.md](desks/BUILD.md)'s boxes plus the ones the workspace adds. That page's sixth box — the seat model on the shared hand — stays empty here too, and it stays empty until Michael's go.

- [ ] Seat page, body, and desk on disk, same slug — the five boxes a person can check today on [desks/BUILD.md](desks/BUILD.md) all pass first.
- [ ] **Its workspace folder exists**, contains exactly the five files, and contains no `MEMORY.md`.
- [ ] **It can say who it works for and who fills it** — Michael Drew, and "not recorded" unless it is the COO.
- [ ] **It can name its own hands and its own denials out loud**, and they match its row on [runtime-body.md](runtime-body.md).
- [ ] It opened its own router folder in [skills/](../skills/README.md) without the PA writing the page for it.
- [ ] It took one named leftover and finished it, or said the queue is honestly empty and named where it looked.
- [ ] It handed the finished thing to its owner's chat and stopped.
- [ ] **Nothing was sent, no channel is bound, and no skill was fetched from a registry.**

All eight is a worker. Seven is a good folder.

## What this repo genuinely cannot check

Everything above the machine line. This repo is markdown ([README.md](../README.md)). It cannot see whether OpenClaw is installed, whether a workspace directory exists, or whether a channel got bound by accident. Those get confirmed at the M1, on [desks/BUILD.md](desks/BUILD.md), by a person looking at the machine.

And one gap the engine does not close by existing, already written down on [bodies/README.md](bodies/README.md): **a body handed to a model has no files and no browser.** It cannot open [offers.md](offers.md), [clients.md](clients.md), or a Notion page by itself, so a job that needs one of those gets "not in hand — open the page" and a person opens it. Closing that is the honest reason anyone would want a gateway at all, and it is not closed today.

## Leftovers

- Michael says whether OpenClaw is ever installed on this M1 at all. Until he does, this folder is source, not a plan, and nobody is named as the one who would stand it up.
- The shared hand waits on Michael's go, and how it is actually loaded — tag, context size, call settings — is named missing in [SOURCES.md](../SOURCES.md) rather than guessed here.
- Slack is connected and no seat's job sources it. Michael names the job, or it stays unused — no workspace here reaches for it.
- If a workspace is ever stood up for real, OpenClaw's own advice is to keep it in a **private** git repo, because it becomes that seat's memory. This repo is not that repo, holds no memory, and should not become the backup for one. That advice is not theoretical: [sententialpeet/boslab-workspace](https://github.com/sententialpeet/boslab-workspace) is somebody's live workspace left public, and what leaked with it is workspace state, server logs, pid files, and a virtualenv sitting beside the operating files.

## What we reused

Searched public GitHub and the public registry first, per [reuse-what-github-has](../skills/reuse-what-github-has/SKILL.md). Everything below is public, and none of it is a Platformology program repo:

- [openclaw/openclaw](https://github.com/openclaw/openclaw) and [docs.openclaw.ai/concepts/agent-workspace](https://docs.openclaw.ai/concepts/agent-workspace) — the workspace file map, the "treat it as memory" framing, the `AGENTS.md`-for-rules / `SOUL.md`-for-voice split, the `USER.md` dated-directive convention and its 4,000-character budget, `BOOTSTRAP.md` as a one-time ritual you delete, the per-agent workspace resolution, the switch that stops the runtime seeding its own bootstrap files, and the private-git-backup advice. Its channels, pairing, streaming, agent-to-agent messaging, sandboxes, and installer were read and deliberately **not** adapted — they are the send path this repo locks.
- [docs.openclaw.ai/concepts/soul](https://docs.openclaw.ai/concepts/soul) — voice in one short file, operating rules kept out of it.
- Read and **not** adapted: [docs.openclaw.ai/concepts/model-providers](https://docs.openclaw.ai/concepts/model-providers). Its one-server-many-agents shape is the one [bodies/README.md](bodies/README.md) already records, so nothing was taken from it, and every provider tag, base URL, and setting on that page stayed there. This page carries no tag.
- [clawhub.ai](https://clawhub.ai) and [docs.openclaw.ai/clawhub](https://docs.openclaw.ai/clawhub) — the public registry, read for what genuinely exists per seat and then refused for install. Details and the full per-seat list: [clawhub-list.md](engine/clawhub-list.md).
- [sententialpeet/boslab-workspace](https://github.com/sententialpeet/boslab-workspace) — a live OpenClaw workspace left public. Unlicensed, so nothing was copied from it; it was read as evidence. It confirms the file set above is a real convention, its dated memory logs are the argument for writing none of ours, and its public state files are the argument for the private-repo leftover below.

The rows are in [SOURCES.md](../SOURCES.md). No client, price, person, KPI, or machine fact came from any of it — the facts on this page are Michael's word or already recorded in this handbook.
