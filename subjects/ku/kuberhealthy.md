# kuberhealthy

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kuberhealthy/kuberhealthy, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/kuberhealthy

## Pinned environment

- Project commit: `ab3f163197f8350289c0f91baab9f42096632e05`
- Test commit: `ab3f163197f8350289c0f91baab9f42096632e05`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.8 to 12.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 12.8 | 1 | 1 | [run](https://argusic.com/run/ed5bc187-ca68-443e-b685-ae05990be144) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go (golang) compiler not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
