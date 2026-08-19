---
name: reuse-what-github-has
description: Before writing a new process, handbook page, or skill for Platformology, search public GitHub first and adapt an existing pattern — name every repo and file reused, and leave any real gap named as missing. Use whenever asked to write a new SOP, handbook page, or skill.
---

# Reuse what GitHub already has

Reused from: the open Agent Skills `SKILL.md` convention documented at [ItamarZand88/awesome-agent-conventions](https://github.com/ItamarZand88/awesome-agent-conventions/tree/main/conventions/skill-md) (frontmatter + procedural body, one repo/file cited per capability), and [llodev/skills](https://github.com/llodev/skills), `docs/publishing-guide.md` (a skill is a folder with attribution, not an invention). This is the same method used to build this whole repo — see [`SOURCES.md`](../../SOURCES.md).

## When to use this
Someone asks for a new SOP, a new handbook page, or a new skill for Platformology.

## Steps
1. Search public GitHub first. Try the obvious repo names, plus plain-English search terms for the job (e.g. "offer ladder SOP," "last-gate QC," "FAQ gate support reply").
2. Read at least two or three candidates before writing anything.
3. Pick the one whose **structure and phrasing** fit — not the one with the most features.
4. Adapt the shape: headings, checklist style, table format. Do **not** copy anyone's invented company, prices, clients, KPIs, or C-suite.
5. Name what you reused — repo plus exact file path — at the top of the new file, and add it to [`SOURCES.md`](../../SOURCES.md).
6. Fill the adapted structure with only sourced Platformology facts (`handbook/`) or Michael's direct word. Wherever a fact is missing, write it down as missing — in the file and in `SOURCES.md` — instead of guessing.
7. Run the result through [`reviews/last-gate-checklist.md`](../../reviews/last-gate-checklist.md) before it ships.

## Never
- Never invent a framework, a persona, or a company fact because a public template had one.
- Never skip the search step because "I already know how to write this."
- Never leave a reused file uncredited in `SOURCES.md`.
