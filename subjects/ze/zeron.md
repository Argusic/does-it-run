# zeron

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zeronsh/zeron, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/zeron

## Pinned environment

- Project commit: `1fdcfe19ac9c758f9df994d288fb362b16fb39b8`
- Test commit: `1fdcfe19ac9c758f9df994d288fb362b16fb39b8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 32.1 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/d14bc241-a291-4f9a-88e9-035f18e8a69e) |
| 2 | pass | 100 | 26 | 32.1 | 4 | 4 | [run](https://argusic.com/run/d33a52fe-87f9-418c-8dad-fad3ac66fdb3) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `systemd user service unavailable (no user bus)`
- 6 min: `edge vitest/wrangler require Node>=20/22, container had Node 18`
- 8 min: `full zeron GUI source build failed on missing fontconfig.pc dev package (no root)`
- 4 min: `e2e-smoke driver got 401 on IPC (prebuilt 0.3.20 vs source driver 0.2.90 skew)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
