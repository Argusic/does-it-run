# deja

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/geo-fer/deja, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/run/6efb37fe-8dc1-42e5-9102-9d1997dc8381

## Pinned environment

- Project commit: `1ee2074be3cabe2859179b314f72469d700dec1d`
- Test commit: `1ee2074be3cabe2859179b314f72469d700dec1d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.5 to 4.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 4.5 | 1 | 1 | [run](https://argusic.com/run/6efb37fe-8dc1-42e5-9102-9d1997dc8381) |
| 2 | pass | 100 | 2.5 | 2.5 | 0 | 0 | [run](https://argusic.com/run/55224ef8-fe20-4329-94a1-7adf34867515) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
