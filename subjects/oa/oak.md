# oak

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/oakmound/oak, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/oak

## Pinned environment

- Project commit: `ae327857d9b97c90bf0e133db5b91616baae9527`
- Test commit: `ae327857d9b97c90bf0e133db5b91616baae9527`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.3 to 23.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 23.3 | 3 | 3 | [run](https://argusic.com/run/b3ae0092-9d0d-45b1-b841-b7bbeca371b6) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Go compiler not pre-installed in container`
- 2 min: `audio tests fail: pcm.Init: default is not supported on this platform`
- 1 min: `examples/text needs go mod tidy due to go version mismatch (go 1.18 -> 1.26)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
