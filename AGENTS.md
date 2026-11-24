<!-- ai-standard: v2026-11-23 (roy-elia/ai-standards). Canonical router: CLAUDE.md imports this file. -->
# alcaraz-attack-policies: working rules for coding agents

## 1. What this repo is
Static pages (plain HTML and one CSS file, no build step) that publish the privacy policy, terms of service and OAuth callback landing page for the Alcaraz Attack Pipeline tool.
- Type: code project (static site)
- Owner of this file, skills and structure: roy-elia (solo repository)
- Integration branch: `main` (never commit to it directly; branch, then pull request)
- Systems of record: the pipeline project lives in the AlcarazAttackPipeline repository; no tracker, wiki or hosting target is recorded here (see Owner questions)

## 2. Resolve context before acting
1. Read `docs/INDEX.md`, then only the page you will change.
2. If a handoff exists, read `state/alcaraz-attack-pipeline-policies/HANDOFF.md` first (created on first use).
3. If something needed is missing, say so and ask. Do not guess.

## 3. Document index
| Need | File | Read when |
|---|---|---|
| Where files go, sources of truth | `docs/INDEX.md` | Placing or finding any file |
| Landing page, links to policies | `index.html` | Changing navigation or the site title |
| Privacy policy | `privacy.html` | Changing data-handling statements |
| Terms of service | `terms.html` | Changing terms |
| OAuth callback landing page | `callback/index.html` | Changing the page OAuth redirects to |
| Shared styles | `style.css` | Changing layout or typography |

## 4. Task-to-context routing
| Request type | Read first | Load if needed |
|---|---|---|
| Edit policy wording | `privacy.html` or `terms.html` | `index.html` (repeats effective dates) |
| Change OAuth callback or styling | `callback/index.html` or `style.css` | none |

## 5. Where things go
Pages sit at the repo root; the callback page is `callback/index.html`. Full table in `docs/INDEX.md`. If no row fits, ask before creating a new location.

## 6. People and owners
roy-elia (@roy-elia) owns everything (solo repository).

## 7. Rules
- Git: never commit or push automatically; suggest it and wait. Work on a short-lived branch.
- Publishing: this site is public. Never publish or deploy; a human does.
- Do not remove or alter the `google-site-verification` meta tag in `index.html`; it proves site ownership.
- Policy text is a legal-style public statement: change it only when asked, and keep effective dates consistent between `index.html` and the policy pages.
- No secrets, tokens, emails or personal data in any page. Contact stays the GitHub profile link already in the pages.

## 8. Skills catalog
None: this repo has no skills.

## 9. Commands
| Task | Command |
|---|---|
| Preview locally | open `index.html` in a browser (no build step) |
| Health check (standard) | `bash .github/scripts/ai-health-check.sh` |

## 10. Conventions
- Plain HTML and CSS only; no frameworks or build tooling were found in the repo.
- Every tracked Markdown file under `docs/` has front matter (`owner`, `status`, `last_updated`, `source_of_truth`).

## 11. More detail
- `docs/INDEX.md`: read when placing or finding a file.
- Standard this repo follows: roy-elia/ai-standards `standard.md` (read when changing structure).

## Owner questions
- Where is the site hosted (the repo has no deploy config), and what is its public URL?
- Should the page titles keep the Alcaraz name now that the pipeline has a Six Star sibling?
