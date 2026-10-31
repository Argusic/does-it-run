# chroma-go

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amikos-tech/chroma-go, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/chroma-go

## Pinned environment

- Project commit: `5cdd8ea46417ec8d752946862f1c070225e5184a`
- Test commit: `5cdd8ea46417ec8d752946862f1c070225e5184a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19.8 to 19.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 19.8 | 2 | 2 | [run](https://argusic.com/run/56f650c3-4c09-4fca-81ae-de0ec18ab947) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `setOfflineRuntimePathOrSkip picked the providers plugin library instead of the main libonnxruntime.so.1.23.1 because the *.so glob missed versioned files and the plugin sorted alphabetically last`
- `6 integration tests (TestClientHTTPIntegration*, TestCollectionAddIntegration) fail because Docker is not available in the container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
