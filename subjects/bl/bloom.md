# Bloom

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Li-Evan/Bloom, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/bloom

## Pinned environment

- Project commit: `b3918981bb34ef5d3090dc81cc5b184555ae3bd6`
- Test commit: `b3918981bb34ef5d3090dc81cc5b184555ae3bd6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3.5 | 3.4 | 3 | 3 | [run](https://argusic.com/run/e690a0b3-584f-4e68-97f3-3590a118b519) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `'uv' not installed, 'source' not available in sh`
- 0.5 min: `Test assertion: brittle ordering in test_refresh_keeps_saved_list_and_replaces_suggestions`
- 1.5 min: `Node.js 18.19.1 too old for Vite 8 (requires ≥20.19)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
