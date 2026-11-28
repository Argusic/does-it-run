# mofa

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mofa-org/mofa, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/mofa

## Pinned environment

- Project commit: `e98f87f6462c360b9096933d3c4c971c1b5cf0e5`
- Test commit: `e98f87f6462c360b9096933d3c4c971c1b5cf0e5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 12.7 to 46.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 46.6 | 0 | 0 | [run](https://argusic.com/run/bbf95a08-14fd-41dd-8e59-c3305d632345) |
| 2 | pass | 100 | 2.5 | 12.7 | 0 | 0 | [run](https://argusic.com/run/9d376277-d53e-42de-b0ed-8bcf69ca9dd4) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
