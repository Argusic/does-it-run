# myPKA

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/myICOR/myPKA, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mypka

## Pinned environment

- Project commit: `9b31da920c2a99269de33e6d64b3c042bc2ec7b8`
- Test commit: `9b31da920c2a99269de33e6d64b3c042bc2ec7b8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 7 | 3 | 3 | [run](https://argusic.com/run/b50f932c-465d-4757-b379-1a74096fbbfa) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `The full red-test suite (run-red-tests.py) cannot run from a standalone myPKA checkout , it requires a combined ICOR for Life + myPKA deployment (mode A or B). This is by design and documented in the code at line 117-130. Exit 2, no FAIL li`
- `check-icor-concepts.py requires source root at /work/icor-for-life (sibling directory) which does not exist in this checkout. Exit 2.`
- `check-version-bump.py requires --base to be a git ref/commit reachable in the repository. No tags exist in this checkout (shallow/fresh clone). Exit 2.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
