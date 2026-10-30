# JoyCode2Api

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vibe-coding-labs/JoyCode2Api, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/joycode2api

## Pinned environment

- Project commit: `176ca9d4d7f98e46a5d979be4cd61b4bc0470b0f`
- Test commit: `176ca9d4d7f98e46a5d979be4cd61b4bc0470b0f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.8 to 16.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 16.8 | 2 | 2 | [run](https://argusic.com/run/338de3c6-00dd-432a-b9ad-585d9668dbef) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.25+ not found in container`
- 4 min: `TestOpenAPIEndpoints/v1_models returned 500 (no upstream mock)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
