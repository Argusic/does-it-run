# flowctl

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cvhariharan/flowctl, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/flowctl

## Pinned environment

- Project commit: `d55e591a0dfe9294af131611aaa2561b33cb52e5`
- Test commit: `d55e591a0dfe9294af131611aaa2561b33cb52e5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.7 to 10.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 10.7 | 6 | 6 | [run](https://argusic.com/run/cfeb5996-e10e-45cd-ba5a-09a242ea4426) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go not installed in container`
- 1 min: `Build failed: //go:embed all:site/build requires site/build directory`
- 2 min: `PostgreSQL not installed`
- 1 min: `libpq.so.5 missing at runtime`
- 1 min: `PostgreSQL failed to start: could not create lock file in /var/run/postgresql`
- 1 min: `Config validation failed: missing required fields`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
