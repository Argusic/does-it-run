# pneumaticworkflow

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pneumaticapp/pneumaticworkflow, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/pneumaticworkflow

## Pinned environment

- Project commit: `e6f1231af0c18fc62d74e3f24afb3b4e7444e0f3`
- Test commit: `e6f1231af0c18fc62d74e3f24afb3b4e7444e0f3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.2 to 18.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 18.2 | 3 | 3 | [run](https://argusic.com/run/3fde1f07-f769-4251-8336-e62f83342fe7) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `Python 3.9 required but only Python 3.12 available; pinned deps missing wheels for 3.12`
- 5 min: `PostgreSQL required but not installed in container`
- `38 tests failed due to django.utils.six and celery EntryPoints compatibility with Python 3.12`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
