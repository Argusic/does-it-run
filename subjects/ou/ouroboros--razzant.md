# ouroboros

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/razzant/ouroboros, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/1741e5ae-9ce8-47a1-a4aa-9bd759350883

## Pinned environment

- Project commit: `796f2e8708ee375216783a7fd80a3bf79f081079`
- Test commit: `796f2e8708ee375216783a7fd80a3bf79f081079`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 53.8 to 53.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 53.8 | 1 | 1 | [run](https://argusic.com/run/1741e5ae-9ce8-47a1-a4aa-9bd759350883) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `rsync not installed in container , test_agency_direct_targets.py rsync parameterized cases fail AssertionError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
