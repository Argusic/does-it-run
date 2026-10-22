# Async

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/x-man-git/Async, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/run/9e27a61f-1467-45b6-aba7-f888414af618

## Pinned environment

- Project commit: `2c18a43c0711d1f991a6eabd913831f9c82794b0`
- Test commit: `2c18a43c0711d1f991a6eabd913831f9c82794b0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 42.1 to 42.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 52 | 42.1 | 2 | 1 | [run](https://argusic.com/run/9e27a61f-1467-45b6-aba7-f888414af618) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `npm run build (chain) aborts: scripts/sync-builtin-team-repo.mjs exits 1 (source repo 'agency-agents' not present in container; only .md docs are synced from it)`
- `npm install exit path; npx first-check failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
