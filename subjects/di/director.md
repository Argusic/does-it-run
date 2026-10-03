# Director

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/video-db/Director, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/director

## Pinned environment

- Project commit: `70e0b3dfdf59c679a25f4bea511e3cc4c5f2457f`
- Test commit: `70e0b3dfdf59c679a25f4bea511e3cc4c5f2457f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16 to 16 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 16 | 2 | 2 | [run](https://argusic.com/run/ad427969-a03a-40b5-9691-280d55b572a9) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `get_default_llm() falls through to VideoDBProxy which validates VIDEO_DB_API_KEY - empty key crashes /agent/ endpoint`
- 3 min: `VideoDB connect() requires a live API server for collection/video operations - without it, /videodb/ endpoints crash`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
