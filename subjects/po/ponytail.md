# ponytail

**Verdict: runs.** Argusic Score 98 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DietrichGebert/ponytail, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ponytail

## Pinned environment

- Project commit: `2ed6c52c9d7e5e56942508591085fd45dea277d3`
- Test commit: `2ed6c52c9d7e5e56942508591085fd45dea277d3`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 4; wall time 1.8 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 7 | 1 | 1 | [run](https://argusic.com/run/d3155a33-4913-4de7-9b2e-5a3c5ec95f8b) |
| 1 | pass | 100 | 0.2 | 1.8 | 1 | 1 | [run](https://argusic.com/run/cf29a14c-4aec-4897-bdf6-df5f097523bc) |
| 2 | pass | 100 | 8 | 3.5 | 1 | 1 | [run](https://argusic.com/run/4b40ca33-32ed-477a-80ba-37bdbf756dce) |
| 3 | pass | 100 | 0.2 | 3 | 1 | 1 | [run](https://argusic.com/run/d7c394fd-2171-44b3-91ee-63dbfa5a572d) |

## What was observed on a clean machine

Attempt 1:

- `csv: correct pandas one-liner passes test failed - pandas Python package not installed`

Attempt 1:

- 0.2 min: `Missing Python dependency: pandas not installed`

Attempt 2:

- 4 min: `pandas not installed , csv correctness test failed`

Attempt 3:

- 0.2 min: `csv correctness test failed because pandas was missing from system Python`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
