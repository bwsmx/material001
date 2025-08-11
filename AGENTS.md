# AGENTS.md – People Counter

## What this repo is
A single-page, offline-first people counter (index.html + inline JS/CSS).

## Rules of engagement
- Do NOT break the primary guard UI: 44+ px touch targets, high contrast, works offline.
- Maintain existing keyboard shortcuts (E, X, U, R).
- If you add files, keep it zero-build (plain HTML/JS/CSS). No bundlers.

## How to run / test
- Serve locally: `python3 -m http.server 8000` and open http://localhost:8000
- Smoke test: page loads; + / – buttons update counts; settings dialog opens with PIN 1234 (configurable).
- If you update storage keys, include a one-time migration and don’t lose prior settings.

## PR requirements
- Update README with any user-facing change.
- Keep changes minimal, focused, and explain *why* in the PR body.

## Backlog hints
- Add GitHub Pages CI.
- Add basic Playwright smoke test (later).
- Add JSON import/export for settings for quick device setup.
