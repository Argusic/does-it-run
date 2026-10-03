# cheat.sh

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chubin/cheat.sh, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/cheat-sh

## Pinned environment

- Project commit: `031a5d3887f035aaa3bf1a3f83dff4fde2aac53d`
- Test commit: `031a5d3887f035aaa3bf1a3f83dff4fde2aac53d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 7.7 to 21.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 7.7 | 2 | 2 | [run](https://argusic.com/run/16700e15-9d24-4a77-a37c-52cf2b44bee7) |
| 2 | pass | 100 | 17 | 21.4 | 5 | 5 | [run](https://argusic.com/run/7e41e101-fe37-456a-9f4a-2bef224eb399) |
| 3 | pass | 100 | 18 | 16.2 | 1 | 1 | [run](https://argusic.com/run/49fa7651-1a6f-40ac-8a8d-862636d40955) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PyICU/polyglot build fails without ICU dev headers (libicu-dev and pkg-config missing)`
- 1 min: `Redis not available`

Attempt 2:

- 3 min: `ModuleNotFoundError: polyglot (PyICU dep) in lib/adapter/question.py`
- 2 min: `AttributeError: NoneType object has no attribute get in frontend/ansi.py`
- 2 min: `learnxinyminutes-docs repo only has .md files but adapter expects .html.markdown`
- 1 min: `Test fixtures stale - upstream repos have evolved since test snapshots created`
- 3 min: `PyICU/polyglot/pycld2 cannot be installed (no root for icu-dev libs)`

Attempt 3:

- 5 min: `PyICU cannot be built: no ICU development headers (libicu-dev, icu-devtools) on system, no root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
