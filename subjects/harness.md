# harness

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/harness/harness, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/harness

## Pinned environment

- Project commit: `ee300c8649011ab2e7f60c0341fe8adbe1e3e3c9`
- Test commit: `ee300c8649011ab2e7f60c0341fe8adbe1e3e3c9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 14 | 3 | 3 | [run](https://argusic.com/run/ebcfcb50-fbed-477a-8323-6398b3ef59a3) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `npm install failed due to peer dependency conflicts with Node 18`
- 2 min: `go:embed web/dist/* failed because webpack build was killed (OOM)`
- `webpack production build killed by OOM (770MB RAM available)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
