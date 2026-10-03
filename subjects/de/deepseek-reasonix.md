# DeepSeek-Reasonix

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/esengine/DeepSeek-Reasonix, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/deepseek-reasonix

## Pinned environment

- Project commit: `61750da510c449f5926f2a20b5ae9d4a1da04431`
- Test commit: `61750da510c449f5926f2a20b5ae9d4a1da04431`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 12.1 to 29.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 25 | 29.7 | 3 | 3 | [run](https://argusic.com/run/a18d2420-8dcc-4ad2-b28d-784857424a8b) |
| 2 | pass | 100 | 3 | 12.1 | 0 | 0 | [run](https://argusic.com/run/376a3c58-8720-46d7-9aad-65e8cb60c2ca) |
| 3 | pass | 100 | 0.5 | 18.9 | 2 | 2 | [run](https://argusic.com/run/7573da44-f301-42b7-ba57-15c1c8c71718) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.26.6 not installed in container`
- `Permission denied installing Go to /usr/local`
- 4 min: `DEEPSEEK_API_KEY missing - no real provider`

Attempt 3:

- 0.5 min: `go: not found - Go toolchain missing`
- 1 min: `TestLoadIncludesStableGlobalPreferencesAndFeedback flaky: pinned guidance sort order flips when alpha-user and zeta-feedback get identical timestamps`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
