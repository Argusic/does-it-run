# Easel

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ZJU-REAL/Easel, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/easel

## Pinned environment

- Project commit: `ed05c2b188933475446823a28814cc4bf4537eed`
- Test commit: `ed05c2b188933475446823a28814cc4bf4537eed`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 20.7 to 20.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 20 | 20.7 | 4 | 4 | [run](https://argusic.com/run/26bbc2f2-a27c-429e-aa5f-1d5bcb9fdfee) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Node.js 18.19.1 too old (OpenClaw requires 24.16+)`
- 2 min: `Python environment externally-managed (Debian), pip install failed`
- 3 min: `npm install -g openclaw used system node (18.19.1) not our Node 24`
- `test_bootstrap_requires_both_env_and_route fails when .env has EASEL_CHAT_TRANSPORT=api (test isolation gap)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
