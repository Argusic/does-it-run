# noodle

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wilfredinni/noodle, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/noodle

## Pinned environment

- Project commit: `384caefa8ea325393e57f15b8c84b603e525d854`
- Test commit: `384caefa8ea325393e57f15b8c84b603e525d854`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.3 to 9.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 29 | 9.3 | 3 | 3 | [run](https://argusic.com/run/579e0cdf-3ae3-4fac-8fe5-025e991eb314) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `bun: not found , bun binary not pre-installed`
- 1 min: `unzip: not found , official bun.sh install script failed`
- 3 min: `test CollectionRunnerView > completes home and collection data paths: completion never appears because collapseUserPath returns absolute path unchanged when repo is outside $HOME`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
