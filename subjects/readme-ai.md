# readme-ai

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eli64s/readme-ai, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/readme-ai

## Pinned environment

- Project commit: `6f507b5f87795799649cfe5eb78d8644f8c2eac8`
- Test commit: `6f507b5f87795799649cfe5eb78d8644f8c2eac8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.4 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 5.4 | 5 | 5 | [run](https://argusic.com/run/a75b5079-d648-42bc-b23b-ce263905188c) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `tiktoken failed to build from source (no Rust compiler)`
- 1 min: `poetry.core.masonry.api missing for editable install`
- 3 min: `Missing click and other runtime deps (dependency resolver didn't install them due to version conflicts)`
- 1 min: `Missing optional google-generativeai package`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
