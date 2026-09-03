# encode/django-rest-framework context
> refreshed 2026-09-02 | upstream default: main @ ae9fd0c7

## Identity & policies
- upstream: encode/django-rest-framework, default branch main, primary language Python, English-first (yes)
- CLA/DCO: none
- AI-assisted PR policy: unstated (no ban, no disclosure requirement found)
- signed commits required: no
- PR template: PULL_REQUEST_TEMPLATE.md (repo root) — simple Description template, link issues with `refs #...`
- external tracker: github
- CONTRIBUTING: feature-complete project. "Apart from minor documentation changes, the GitHub discussions page should generally be your starting point. Please only open a pull request if you've been recommended to do so after discussion." => docs fixes are the discussion-free contribution type.

## Conventions (verified from merged PRs)
- branch naming: mixed — `fix/...`, `docs-...`, `update/...`, `patch-N`, `codex/...`; no dominant single pattern
- commit style: plain imperative subject, no conventional-commit prefix, PR number in parens
- test command: `pytest` (tox envlist py310-314 x django52-61); `pip install -e . --group dev`
- CI: GitHub Actions; pre-commit/prek lint
- outside PRs DO get merged: recent external merges (epuronta, abidaliamanat9, peterthomassen, Ernest0x, vishalanandl177, harshitkandpal) reviewed by browniebroke/auvipy. Docs fixes merge readily.

## Maintainer picture
- active maintainers: browniebroke, auvipy (reviewers); responsive (docs PRs merged within days)
- in-flight: Django 6.1 support, release prep

## Issue-area health
- Issue #5236 (TemplateHTMLRenderer list crash) is ALREADY FIXED by merged PR #9467 (2024-07-15) — `get_template_context` returns `{'details': data, ...}` for list data. Remaining thread discussion (change 'details'->'results') is a design question NOT accepted by maintainers. NOT a pick.
- Open issues are mostly unlabeled/unconfirmed or "Needs design decision" — no maintainer-engaged/approved open issue survives.

## Gap ledger (dedupe — READ FIRST, never re-pick)
- 2026-09-02 issue #5236 — dropped (already fixed by merged PR #9467; remaining 'details'->'results' is unaccepted design change)
- 2026-09-03 trivial-fix pass — 3 verified broken-link fixes bundled into ONE docs PR (fork PR #2): (1) project-management.md release-notes link pointed to blob/mains (typo) + old docs/topics/ path, file now at docs/community/release-notes.md; (2) rest-hypermedia-hateoas.md steveklabnik reading-list link dead, replaced with current URL; (3) release-notes.md contributor link @maerteijn 404, account renamed to mj026 (same user, PR #9198). All replacements verified 200. Fork CI: Actions enabled but 0 workflows registered, no checks appear (fork artifact).

## Mined gaps (discovered, not yet attempted)
- (to be filled by repo-audit)
