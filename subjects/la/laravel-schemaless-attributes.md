# laravel-schemaless-attributes

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spatie/laravel-schemaless-attributes, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/laravel-schemaless-attributes

## Pinned environment

- Project commit: `36fc2b8ae638c4bfe5300cb7ec875ba969370bb8`
- Test commit: `36fc2b8ae638c4bfe5300cb7ec875ba969370bb8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 5 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 8.1 | 2 | 2 | [run](https://argusic.com/run/5ca2458d-7359-4f73-be7e-dbbbe36642b7) |
| 2 | pass | 100 | 15 | 5 | 2 | 2 | [run](https://argusic.com/run/288edbc9-1826-4b40-a6c0-eb170c5dfcf6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No PHP runtime in container`
- 2 min: `No MySQL server available - tests failed with connection refused`

Attempt 2:

- 4 min: `No PHP runtime installed in container (needed PHP ^8.0 for composer/laravel)`
- 3 min: `No MySQL server available in the container for test suite database`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
