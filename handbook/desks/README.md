# Sit down and run a seat

This is the page you open first. Pick your seat in the table, open its desk file, and do what that file says. You do not need anyone to tell you what to click after that.

**No send without Michael.** Every draft, quote, and reply stops with him. That is true for every row below, including the parked and unassigned ones.

Platformology LLC is one company with two names the public sees: Promote a Book and Book Retreat. You are sitting in a seat, not becoming a person, and you are not installing a model to do this job. The lock list is [locks.md](../locks.md). Read it before you touch a client message, a price, or a repo.

## What you do

1. Read [locks.md](../locks.md).
2. Find your seat in the table. The **Desk** column is the pack you sit down with.
3. Open that file and follow it in order.
4. If you are on the office Mac (the M1), the **On the M1** column is the command that calls the shared local hand for that seat. One shared hand, twenty-three names. Thinking stays off.
5. When the pass is done, run [reviews/last-gate-checklist.md](../../reviews/last-gate-checklist.md). Then stop. Nothing leaves without Michael.

You do not need a model to run a desk. The desk file plus the pages it names are enough. The M1 command is only if you are already on that machine and the alias is already built.

## The twenty-three seats

| Seat | Status | Desk | On the M1 |
|---|---|---|---|
| PA | Assigned | [pa.md](pa.md) | `ollama run pa --think=false` |
| COO | Assigned | [coo.md](coo.md) | `ollama run coo --think=false` |
| CMO | Assigned | [cmo.md](cmo.md) | `ollama run cmo --think=false` |
| Head of Content | Assigned | [head-of-content.md](head-of-content.md) | `ollama run head-of-content --think=false` |
| Head of Demand | Unassigned | [head-of-demand.md](head-of-demand.md) | `ollama run head-of-demand --think=false` |
| CSO | Assigned | [cso.md](cso.md) | `ollama run cso --think=false` |
| Head of Sales | Unassigned | [head-of-sales.md](head-of-sales.md) | `ollama run head-of-sales --think=false` |
| SDR | Unassigned | [sdr.md](sdr.md) | `ollama run sdr --think=false` |
| CFO | Assigned | [cfo.md](cfo.md) | `ollama run cfo --think=false` |
| Controller | Assigned | [controller.md](controller.md) | `ollama run controller --think=false` |
| Bookkeeper | Assigned | [bookkeeper.md](bookkeeper.md) | `ollama run bookkeeper --think=false` |
| CTO | Assigned | [cto.md](cto.md) | `ollama run cto --think=false` |
| Head of Engineering | Parked | [head-of-engineering.md](head-of-engineering.md) | `ollama run head-of-engineering --think=false` |
| Developer | Parked | [developer.md](developer.md) | `ollama run developer --think=false` |
| CCO | Assigned | [cco.md](cco.md) | `ollama run cco --think=false` |
| Head of Author Success | Assigned | [head-of-author-success.md](head-of-author-success.md) | `ollama run head-of-author-success --think=false` |
| Client Success | Assigned | [client-success.md](client-success.md) | `ollama run client-success --think=false` |
| CHRO | Assigned | [chro.md](chro.md) | `ollama run chro --think=false` |
| People Ops | Assigned | [people-ops.md](people-ops.md) | `ollama run people-ops --think=false` |
| VP Campaigns | Assigned | [vp-campaigns.md](vp-campaigns.md) | `ollama run vp-campaigns --think=false` |
| Campaign Coordinator | Assigned | [campaign-coordinator.md](campaign-coordinator.md) | `ollama run campaign-coordinator --think=false` |
| VP Retreats | Assigned | [vp-retreats.md](vp-retreats.md) | `ollama run vp-retreats --think=false` |
| Retreat Producer | Assigned | [retreat-producer.md](retreat-producer.md) | `ollama run retreat-producer --think=false` |

Assigned seats do the job on their desk. Parked seats (Head of Engineering, Developer) refuse work. Unassigned seats (Head of Demand, Head of Sales, SDR) refuse work and say the seat is unassigned. Do not start Engineering or Developer work from this folder. Do not pick up Demand, Sales, or SDR work to make the chart look busy.

## Before you pick a row

- The seat page in [seats/](../seats/README.md) is the source of truth for what the seat owns. If a body file in [bodies/](../bodies/README.md) says something else, the seat page wins. Conflicts we found are named on the desk and listed in [CONFLICTS.md](CONFLICTS.md).
- The only hands an assigned seat may use are already written in [runtime-body.md](../runtime-body.md). Nothing else gets added. No HubSpot. No Bench pull. No new CRM.
- Prices come from [offers.md](../offers.md), both numbers where that page shows two. Clients come from [clients.md](../clients.md). People come from [people.md](../people.md).
- The M1 is the office. The M5 is the shop only, and it stays parked. Seats are never rebuilt as local models. The local hand, when you call it, is the shared `office-hand` under twenty-three names.

## If you are building the desk, not sitting in it

Open [BUILD.md](BUILD.md). That is the CTO's check-off page for when a seat is fully built on the M1.
