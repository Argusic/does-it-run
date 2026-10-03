# dtm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dtm-labs/dtm, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/dtm

## Pinned environment

- Project commit: `18146ee53bafbf094b1a5f12ca7e8a29bdb57edd`
- Test commit: `18146ee53bafbf094b1a5f12ca7e8a29bdb57edd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.3 to 20.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 20.3 | 1 | 1 | [run](https://argusic.com/run/1eaa2c53-0418-4135-ac9d-7cab738cab82) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.22 not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
