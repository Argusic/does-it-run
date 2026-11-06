# evcc

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/evcc-io/evcc, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/evcc

## Pinned environment

- Project commit: `0972249b9242fc94b11493e7096d080604a353e6`
- Test commit: `0972249b9242fc94b11493e7096d080604a353e6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 9.7 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 14.2 | 0 | 0 | [run](https://argusic.com/run/a8f12ed0-dc73-4a06-9be4-3a3b870fc437) |
| 2 | pass | 100 | 9.5 | 9.7 | 3 | 3 | [run](https://argusic.com/run/5ea3c44f-bc2a-44cf-9a55-0cf016b4030b) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Go 1.27.3 not found on PATH (required by go.mod)`
- 2 min: `Node.js v18.19.1 does not satisfy package.json requirement >=26.0.0, and vp/Vite+ requires newer Node`
- 1.5 min: `vp run build failed: task cache settings require input under cache, run vp migrate`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
