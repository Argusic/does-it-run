# semantix

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Gnosil/semantix, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/semantix

## Pinned environment

- Project commit: `aad62b0b3f3ebdd8c0ed9454e7d5e11e6e603a67`
- Test commit: `aad62b0b3f3ebdd8c0ed9454e7d5e11e6e603a67`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.2 to 17.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 17.2 | 1 | 1 | [run](https://argusic.com/run/1e23a2b3-a739-4529-969b-130e26cdb503) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.26+ not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
