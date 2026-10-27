# znai

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/testingisdocumenting/znai, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/znai

## Pinned environment

- Project commit: `c37ae2e53eae119c566364c19460b153ac0d615f`
- Test commit: `c37ae2e53eae119c566364c19460b153ac0d615f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 40.1 to 40.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 37 | 40.1 | 7 | 7 | [run](https://argusic.com/run/28180cb6-8ca1-4749-947f-27df5983486d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Java not found in container`
- 2 min: `Maven not found in container`
- 1 min: `unzip not installed and no root to install it`
- 3 min: `Firefox not found for WebTau Selenium tests`
- 5 min: `Graphviz dot not found for diagram tests`
- `znai-tests webtau integration tests failed (Firefox missing)`
- `znai-testing-examples webtau tests failed (Firefox missing)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
