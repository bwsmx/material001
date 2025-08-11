# AGENTS.md – People Counter (material001)

## What this repo is
A single-page, offline-first people counter (index.html + inline JS/CSS). Multi-counter, per-counter capacity/lockout, offline queue, optional endpoint sync.

## Branch policy
- Default branch: `dev`. Feature work happens on `dev` or short-lived feature branches.
- Open PRs into `main` for releases. Do NOT push directly to `main`.
- Codex: always open PRs into `main`.

## Guardrails
- Keep the guard UI simple: huge tap targets (≥44px), high contrast, keyboard shortcuts (E=+1, X=−1, U=undo, R=clear).
- Offline-first must never break; localStorage persistence must survive reloads.
- If changing storage keys, include a one-time migration to preserve settings.
- Avoid adding build tooling. Keep plain HTML/JS/CSS unless explicitly requested.

## Testing
- Manual smoke: load index.html, tap +/−, open ⚙️ with PIN (1234 by default), confirm endpoint/counters persist after reload.

## PR requirements
- Keep changes small and focused; explain *why* in PR body.
- Update README for user-visible changes.
