# better-curl-saul

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DeprecatedLuar/better-curl-saul, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/better-curl-saul

## Pinned environment

- Project commit: `4c324567921c9ccc25ea4824711dffd726c97088`
- Test commit: `4c324567921c9ccc25ea4824711dffd726c97088`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.5 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 11 | 5.5 | 3 | 3 | [run](https://argusic.com/run/ef7f7f34-af36-42f1-a963-c0ddb8938c11) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not pre-installed (go: command not found)`
- 1 min: `Python http.server kept dying between shell invocations`
- 2 min: `TestLazyFileCreation failed: env vars SAUL_CONFIG_DIR_PATH/SAUL_APP_DIR_NAME/SAUL_PRESETS_DIR_NAME not respected by config/dirpaths.go`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
