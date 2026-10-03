# curlie

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rs/curlie, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/curlie

## Pinned environment

- Project commit: `5dfcbb17ea673b66a3faab66d2ff5f24145f45a8`
- Test commit: `5dfcbb17ea673b66a3faab66d2ff5f24145f45a8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.2 to 17.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17 | 17.2 | 1 | 1 | [run](https://argusic.com/run/c47cf430-62a0-4014-9c31-f6733b80b000) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not preinstalled in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
