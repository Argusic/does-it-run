# claudemy

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/assafkip/claudemy, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/claudemy

## Pinned environment

- Project commit: `438a6288fa74a2edad2cc86416d28308cb02ee1a`
- Test commit: `438a6288fa74a2edad2cc86416d28308cb02ee1a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 2.3 to 3.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 2.3 | 0 | 0 | [run](https://argusic.com/run/9438c77f-6b54-4bdc-8fc9-a02a25529874) |
| 2 | pass with mocks | 92 | 2 | 3.5 | 1 | 1 | [run](https://argusic.com/run/2ac4984e-db08-4672-86bf-4b3aec261241) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pip3 install beautifulsoup4 failed: externally-managed-environment (PEP 668)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
