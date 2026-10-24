# redux-requests

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/klis87/redux-requests, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/redux-requests

## Pinned environment

- Project commit: `36eff89a778f0d61ce6da6cfb977d3f1023aef23`
- Test commit: `36eff89a778f0d61ce6da6cfb977d3f1023aef23`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11 to 11 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 11 | 3 | 3 | [run](https://argusic.com/run/85e02e06-decf-4855-8974-715753dc9508) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `iltorb native build failed with Python 3.12 (invalid mode 'rU')`
- 0.1 min: `@redux-requests/core not prebuilt (missing lib/)`
- 1 min: `Timing-flaky polling tests due to real setTimeout under parallel load`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
