# Locks

Adapted from the [dswh/company-os](https://github.com/dswh/company-os) `rules.md` never / ask-first pattern. This page is permissions, not culture — nobody, human or bot, edits this list without Michael.

## Never, no exceptions
- **No send without Michael.** Nothing goes to a client, a prospect, or the public without Michael's sign-off.
- **No program GitHub.** This repo is docs only. Do not touch, clone, fork, or open PRs against `smarter-voice`, `academic-research-platform`, `book-campaign-platform`, `styleguide-os`, `persona-standalone-programs`, or `tlpF-b01-research-engine`.
- **No VMs.**
- **No GKE.**
- **No local LLM until Michael says go.** Same trigger as the M5 park: not in hand, not once it is set up, not after a reinstall — until he says go. Until then there is no local model on any machine here. After he says go, models get installed at Phase 4 below, and not a step earlier.
- **Seats are never rebuilt as local models.** That one does not change at go. Installing a model at Phase 4 does not turn a seat into one.
- **The M1 is the office. The M5 is the shop only.** The M1 is the desk this company runs on, and it stays that way. The M5 is a shop machine: it is not the company desk, the office does not move onto it, and Grok Bot does not move onto it.
- **M5 stays parked until Michael says go.** Not until it is in hand, not once it is set up, not after a reinstall — until Michael says go. Nothing here waits on that machine, and the next PA does not start after a reinstall on the M5.
- **Blue Sky stays off the LLC books.**

## Ask Michael first
- Picking a number where the offer ladder shows "both" (see [offers.md](offers.md)).
- Recording a client as Current, Prospect, or otherwise moving them off "question" status (e.g., Hoffman — see [clients.md](clients.md)).
- Choosing between the two unresolved Zoom URLs for the Cornelia Choe meeting.
- Assigning a Role to Jhana or Bob.
- Anything that would change this file.

## When Michael says go
Recorded 19 Aug 2026 — Michael, via the CTO. Nothing below starts until he says go, and it runs in this order:

1. **Phase 1 — clone this M1 onto the M5.**
2. **Phase 2 — the CTO proves the copy.**
3. **Phase 3 — strip this M1 to the office.**
4. **Phase 4 — then install models.** The list is on [When you say go](https://app.notion.com/p/3c125e30d68b81a3b351c0ce17aa4602) (Notion); this page does not restate it. Phase 4 is the only thing that lifts the local-model lock above — no earlier phase does, and neither do **No VMs** or **No GKE**, which stay locked.

Three things hold across all four phases:

- **Nothing is deleted on the M1 until the M5 copy is proven.** Phase 1 is a copy, not a move, and Phase 3 does not begin until Phase 2 passes.
- **After Phase 3 the office is still this M1.** Stripping it to the office is what keeps it the office — it is not what hands the office to the M5.
- **Daily Grok Bot does not live on the M5.** Not before go, not after it.

**Open this in Notion:** [Desk](https://app.notion.com/p/3c125e30d68b81319e5bd9907af3d65e) — which machine is the office · [When you say go](https://app.notion.com/p/3c125e30d68b81a3b351c0ce17aa4602) — what unparking the M5 actually means. Those two pages are the live source; this page does not restate them.

## Why this page exists
A new hire or a bot that skips this page is the failure mode this whole repo exists to prevent. Read it before you touch a client message, a Sales Menu number, or a repo.
