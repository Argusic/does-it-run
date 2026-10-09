# Edge0

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Edge0-AI/Edge0, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/edge0

## Pinned environment

- Project commit: `9a56e4da063bebff79152165891f84663814933f`
- Test commit: `9a56e4da063bebff79152165891f84663814933f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 26.2 to 26.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 26.2 | 1 | 1 | [run](https://argusic.com/run/044bef79-cb45-4a63-834f-7de10b767fa4) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `MLX (Apple Silicon) wheel installs on x86_64 Linux but libmlx.so is missing , all MLX code fails at import`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
