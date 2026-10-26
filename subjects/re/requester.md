# Requester

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kylebebak/Requester, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/requester

## Pinned environment

- Project commit: `e1b49b1de6ef7e94c817caebe59a1e51dd4760b9`
- Test commit: `e1b49b1de6ef7e94c817caebe59a1e51dd4760b9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 7.5 to 12.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 12.9 | 0 | 0 | [run](https://argusic.com/run/c4cea5a7-88f9-46b1-8976-b88f12112f33) |
| 2 | pass with mocks | 92 | 3 | 7.5 | 3 | 3 | [run](https://argusic.com/run/9409ef3e-d8cc-4cc8-9bb7-f5a70fcca730) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `ModuleNotFoundError: No module named 'Requester' (tests fail because Requester package not importable)`
- 1 min: `ModuleNotFoundError: No module named 'urllib3' (deps/ not on sys.path when tests import Requester.core)`
- 1 min: `AssertionError: 'EOF' not found in error message (Python 3.12 changed SyntaxError.msg for unclosed parens)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
