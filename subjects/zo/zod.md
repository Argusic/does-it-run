# zod

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/colinhacks/zod, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/zod

## Pinned environment

- Project commit: `680d19f7d1e042e55934209caeb79bc843b94f44`
- Test commit: `680d19f7d1e042e55934209caeb79bc843b94f44`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 32.6 to 90.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 90.1 | 0 | 0 | [run](https://argusic.com/run/1e0666cc-2439-4027-90fb-181dcb19a943) |
| 2 | pass | 100 | 1.5 | 32.6 | 2 | 2 | [run](https://argusic.com/run/34e12d15-9742-4d02-ba2d-ff5a0df96cb5) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `docs package vitest config fails with ERR_REQUIRE_ESM for std-env`
- 5 min: `File is not defined globally in vitest node environment on Node 24`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
