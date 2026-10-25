# iowow

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Softmotions/iowow, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/iowow

## Pinned environment

- Project commit: `bf76141c5d074fd09205db438c43fb85b7bafb51`
- Test commit: `bf76141c5d074fd09205db438c43fb85b7bafb51`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.4 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.3 | 5.4 | 1 | 1 | [run](https://argusic.com/run/1c5613f6-78f7-4bab-8baa-04710e3c8f06) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `CUnit library not found by pkg-config; test build failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
