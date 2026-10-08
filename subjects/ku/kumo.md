# kumo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sivchari/kumo, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/kumo

## Pinned environment

- Project commit: `b312440d8044aa17ea629991fb4ffa58c5e09a10`
- Test commit: `b312440d8044aa17ea629991fb4ffa58c5e09a10`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 57.5 to 57.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 46.5 | 57.5 | 2 | 2 | [run](https://argusic.com/run/a4f091cf-25f6-44b6-9172-853aa8dae149) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Go (golang) toolchain installed in container`
- 1 min: `Stale lock files from killed build processes blocked subsequent builds`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
