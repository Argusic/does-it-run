# anime

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/juliangarnier/anime, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/anime

## Pinned environment

- Project commit: `01b81be1df6843ccfe0a71c0699a746bf740dd77`
- Test commit: `01b81be1df6843ccfe0a71c0699a746bf740dd77`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.3 to 2.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.4 | 2.3 | 1 | 1 | [run](https://argusic.com/run/013029ca-de11-4061-ae8c-bd8d1c832f51) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `5 Node test failures: V8 optimization status assertion expects 49 but Node 18.19.1 returns 81 for same 'TurboFan optimized' state , V8 version difference`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
