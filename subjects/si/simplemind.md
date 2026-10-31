# simplemind

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kennethreitz/simplemind, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/simplemind

## Pinned environment

- Project commit: `c3d8a0c2741c314948e396a6613e5c320e0da8af`
- Test commit: `c3d8a0c2741c314948e396a6613e5c320e0da8af`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 19.1 to 19.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2.5 | 19.1 | 5 | 5 | [run](https://argusic.com/run/6a56066c-c1d3-48b2-a5bf-a8704c5ed954) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `externally-managed-environment - system Python blocks pip install`
- 1 min: `instructor v2 isinstance check failed against monkeypatched constructors`
- 1.5 min: `Tool-calling tests required multi-round tool call simulation`
- 0.5 min: `Pydantic Settings object rejected direct field assignment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
