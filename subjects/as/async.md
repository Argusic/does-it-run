# Async

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ZYKJShadow/Async, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/async

## Pinned environment

- Project commit: `2c18a43c0711d1f991a6eabd913831f9c82794b0`
- Test commit: `2c18a43c0711d1f991a6eabd913831f9c82794b0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.2 to 8.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 7.2 | 2 | 2 | [run](https://argusic.com/run/71928312-56b5-435e-b716-0412e7f5769e) |
| 2 | pass | 100 | 8.7 | 8.4 | 1 | 1 | [run](https://argusic.com/run/4bf89018-4815-4240-874a-c7e35fc3d3fd) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `sync:builtin-team script failed because agency-agents repo not found at configured/fallback paths`
- 1 min: `SUID sandbox helper not configured correctly (need root to chown chrome-sandbox)`

Attempt 2:

- 1 min: `scripts/sync-builtin-team-repo.mjs exits with code 1 when external 'agency-agents' repo is missing (blocking 'npm run build')`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
