# peddler

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lineofflight/peddler, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/peddler

## Pinned environment

- Project commit: `8fe69f6c3227475f2d0603afdc9533419b5296f9`
- Test commit: `8fe69f6c3227475f2d0603afdc9533419b5296f9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.5 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 6.5 | 4 | 4 | [run](https://argusic.com/run/b9425002-50cc-4601-8899-ef2de4344ed4) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Ruby not found in container`
- 1 min: `zlib extension not compiled into Ruby (needed by rubygems)`
- 1 min: `psych (YAML) extension not compiled into Ruby (needed by rubygems)`
- 1 min: `Generator tests failed: missing selling-partner-api-models checkout`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
