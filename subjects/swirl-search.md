# swirl-search

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/swirlai/swirl-search, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/swirl-search

## Pinned environment

- Project commit: `0506aa5638ae0d53ced849e33ce4aac25bd5ce3d`
- Test commit: `0506aa5638ae0d53ced849e33ce4aac25bd5ce3d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.1 to 11.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 11.1 | 2 | 2 | [run](https://argusic.com/run/5d7a091c-81fe-468d-943b-44b05fbd4f69) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Python 3.12 externally-managed-environment blocks system-wide pip install`
- `redis-server binary not available (no root); Celery/Channels requires Redis`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
