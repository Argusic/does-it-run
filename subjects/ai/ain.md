# ain

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jonaslu/ain, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/ain

## Pinned environment

- Project commit: `654623759ec37914d4df27f9add73efc152ac5e7`
- Test commit: `654623759ec37914d4df27f9add73efc152ac5e7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 13.8 to 18.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 12 | 13.8 | 4 | 4 | [run](https://argusic.com/run/e893cef1-8bb2-4639-90b8-1bdf33bf4295) |
| 2 | pass with mocks | 92 | 17 | 18.8 | 4 | 4 | [run](https://argusic.com/run/7f328416-28c7-4be5-b78f-c88e69927eae) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not installed`
- 2 min: `mock.httpstatus.io DNS failure (3 e2e tests)`
- 3 min: `httpie not installed (wget also missing)`
- 1 min: `Python externally-managed-environment blocked system pip install`

Attempt 2:

- 2 min: `go command not found`
- 3 min: `e2e test host mock.httpstatus.io did not resolve (no DNS)`
- 1 min: `wget binary not found in container`
- 1 min: `httpie binary not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
