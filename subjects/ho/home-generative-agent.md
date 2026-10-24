# home-generative-agent

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/goruck/home-generative-agent, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/home-generative-agent

## Pinned environment

- Project commit: `3cbead48e586bfd4a0f72268c68f327c1b5e79d7`
- Test commit: `3cbead48e586bfd4a0f72268c68f327c1b5e79d7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 19.2 to 19.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 30 | 19.2 | 1 | 1 | [run](https://argusic.com/run/b8a544ae-978d-487d-95ca-102654fdc1c9) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Python 3.14 not available in container , HA 2026.9.3 requires Python >=3.13.2`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
