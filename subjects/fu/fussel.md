# fussel

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cbenning/fussel, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/fussel

## Pinned environment

- Project commit: `08cc8128196e7944fbefe3390c6f122dfdd44be9`
- Test commit: `08cc8128196e7944fbefe3390c6f122dfdd44be9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.7 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 11.7 | 6 | 6 | [run](https://argusic.com/run/947fdcbb-204a-4285-a9f0-2cac5737e4d3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv not found in PATH`
- 1 min: `yarn not found in PATH`
- 2 min: `Node.js v18 incompatible with react-router-dom (needs >=20.0.0) and vite (needs >=22.12.0)`
- 1 min: `test_supported_extensions assertion failed (expected old extension list without .avif)`
- 2 min: `test_main_success FileNotFoundError writing .nojekyll to /test/output`
- 2 min: `JS test files 3/6 failed due to missing _gallery stub data files for vitest import resolution`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
