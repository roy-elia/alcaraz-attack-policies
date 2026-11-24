---
owner: roy-elia
status: active
last_updated: 2026-11-24
source_of_truth: local
tags: [index]
---
# docs index

Purpose: shared, durable context for alcaraz-attack-policies. Read this before placing or finding a file.

There are no other documents in `docs/`; the site pages themselves are listed in `AGENTS.md` section 3.

| File | Summary (one line) | Read when | Owner |
|---|---|---|---|

## Where does X go
| I am producing | Put it in | Owning skill | Tracked |
|---|---|---|---|
| A policy or landing page | repo root, `<name>.html` | manual | Yes |
| A page served at its own path | `<path>/index.html` (as in `callback/`) | manual | Yes |
| Shared styling | `style.css` | manual | Yes |
| A decision and its reasoning | `docs/decisions/YYYY-MM-DD-<topic>.md` (created on first use) | manual | Yes |
| Session handoff | `state/alcaraz-attack-pipeline-policies/HANDOFF.md` (created on first use) | session-handoff | Yes |
| Exploratory draft | `output/` | any | No |
| Scratch | `temp/` | any | No |

## Sources of truth
| Content | System of record | Role of this repo | Link recorded in |
|---|---|---|---|
| Published policy text and pages | This repository | Owner record | none |
| The pipeline these policies describe | AlcarazAttackPipeline repository | Link only | none |
| Tickets and bugs | GitHub Issues on this repository | Link only | Pull request description |

## Rules for this folder
- Every Markdown file here starts with front matter (`templates/front-matter.md` in ai-standards).
