# Scrapling

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/D4Vinci/Scrapling, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/scrapling

## Pinned environment

- Project commit: `458e2a2ac909b3235747ebcdb312b93a1080a10a`
- Test commit: `458e2a2ac909b3235747ebcdb312b93a1080a10a`
- Worker image digest: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.8 to 10.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 10.8 | 1 | 1 | [run](https://argusic.com/run/d1e1ac2b-1c14-423e-b465-047999886cf4) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Playwright/patchright browsers cannot launch: missing system libraries (libnspr4.so)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
