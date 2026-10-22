# gojekyll

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/osteele/gojekyll, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/gojekyll

## Pinned environment

- Project commit: `e4135dfb43762346a89117fb948e2d22489b68cc`
- Test commit: `e4135dfb43762346a89117fb948e2d22489b68cc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.7 to 4.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 4.7 | 2 | 2 | [run](https://argusic.com/run/621dd126-0f6b-40f3-9992-f9224f7816b9) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `go: not found , no Go toolchain installed`
- 2 min: `sass: executable file not found in $PATH , 2 filter tests failed (sassify/scssify)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
