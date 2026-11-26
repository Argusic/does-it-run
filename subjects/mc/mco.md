# mco

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mco-org/mco, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mco

## Pinned environment

- Project commit: `d7fef6c96dca10a3ed0fd7c5ecd505e665ca455e`
- Test commit: `d7fef6c96dca10a3ed0fd7c5ecd505e665ca455e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.08 | 7.1 | 0 | 0 | [run](https://argusic.com/run/3c2ec317-9b2b-4751-adc3-0ff99c3cb780) |
| 2 | pass | 100 | 2 | 2 | 2 | 2 | [run](https://argusic.com/run/2af4d725-147b-43eb-856d-38e19b0b4e93) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pip install -e . failed due to externally-managed Python environment`
- 0.5 min: `npm test failed because npm dependencies not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
