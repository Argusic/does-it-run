# finch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/0x4D31/finch, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/run/8be68082-f245-41dd-9570-585b2591cb80

## Pinned environment

- Project commit: `db48717b488888ac2bfb614e27558b50fd714464`
- Test commit: `db48717b488888ac2bfb614e27558b50fd714464`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.5 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 11.5 | 2 | 2 | [run](https://argusic.com/run/8be68082-f245-41dd-9570-585b2591cb80) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Go 1.24+ not installed on system (no root for apt)`
- 8 min: `TestMapPath/query-no-slash unit test expected wrong value`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
