# elegant

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Pelican-Elegant/elegant, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/elegant

## Pinned environment

- Project commit: `b80ebd51779883426e4f17c066c7a0baaa037e75`
- Test commit: `b80ebd51779883426e4f17c066c7a0baaa037e75`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.1 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 5.1 | 3 | 3 | [run](https://argusic.com/run/bd1c8de8-ecd6-4806-a4e9-dd3e098906c3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `externally-managed-environment blocks system-wide pip install`
- 1 min: `invoke 1.7.1 missing dependencies (lexicon, yaml)`
- 0.5 min: `pelican not in PATH when called by invoke`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
