# sulu

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sulu/sulu, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/sulu

## Pinned environment

- Project commit: `ed0dbfc273e484d42c6e4923a5f84f5f17f891f5`
- Test commit: `ed0dbfc273e484d42c6e4923a5f84f5f17f891f5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 59.2 to 59.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 59.2 | 6 | 6 | [run](https://argusic.com/run/5c588353-e45e-48f8-b19c-b3384e4fd5d5) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP not found in container`
- 2 min: `rokka/imagine-vips requires ext-vips/ext-ffi not in static PHP`
- 4 min: `bin/runtests spawns PHPUnit sub-process with default memory_limit=128M`
- 8 min: `MySQL database required for bundle tests using platform-specific SQL`
- 2 min: `JS tests: @testing-library/jest-dom/extend-expect removed in v6`
- 2 min: `JS tests: transformIgnorePatterns excluded local sulu-* bundles (ESM source)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
