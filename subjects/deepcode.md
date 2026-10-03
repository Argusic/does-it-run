# DeepCode

**Verdict: runs.** Argusic Score 90.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HKUDS/DeepCode, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/deepcode

## Pinned environment

- Project commit: `c0a6a3cb595fe82c76f1c3966919423647d5c462`
- Test commit: `c0a6a3cb595fe82c76f1c3966919423647d5c462`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 3.5 to 12.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 12.8 | 0 | 0 | [run](https://argusic.com/run/b80b2fe9-665f-42e9-a4a1-1c29f82353bb) |
| 2 | pass | 100 | 2 | 3.5 | 0 | 0 | [run](https://argusic.com/run/92897e89-82cd-4534-9afd-d93a63efcce3) |
| 3 | pass with mocks | 72 | 13 | 12.9 | 1 | 0 | [run](https://argusic.com/run/9a1e57f9-9770-4a9b-bec7-14fdbfe1ce93) |

## What was observed on a clean machine

Attempt 3:

- `3 tests fail because verification subsystem spawns python3 -m pytest which resolves to system Python (no pytest installed) rather than the venv Python`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
