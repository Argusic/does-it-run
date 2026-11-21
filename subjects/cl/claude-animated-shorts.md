# claude-animated-shorts

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mromidev/claude-animated-shorts, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/claude-animated-shorts

## Pinned environment

- Project commit: `e3b817b6afc6cd413466d43f11ba31209e034bbf`
- Test commit: `e3b817b6afc6cd413466d43f11ba31209e034bbf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 3.2 to 10.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 3.2 | 2 | 2 | [run](https://argusic.com/run/12ffea79-0f78-4974-809c-ff903f0a962c) |
| 2 | pass with mocks | 92 | 13 | 10.7 | 1 | 1 | [run](https://argusic.com/run/aefba6f8-907d-4d5d-bb4d-27bf1f1a5c12) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing numpy and scipy for audio synthesis scripts`
- 0.5 min: `Missing PIL/Pillow for QA script short_qa.py`

Attempt 2:

- 1 min: `TypeScript unused import errors in cast.ts (fxBlob, LIGHTS)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
