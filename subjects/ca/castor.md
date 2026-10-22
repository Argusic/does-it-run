# castor

**Verdict: runs.** Argusic Score 88.9 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jolicode/castor, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/castor

## Pinned environment

- Project commit: `56cd0342f2d1f0339bf5937a5ea315d5d1b313a8`
- Test commit: `56cd0342f2d1f0339bf5937a5ea315d5d1b313a8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 54.9 to 54.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 88.89 | 35 | 54.9 | 9 | 4 | [run](https://argusic.com/run/c051443a-1d87-401f-bae0-c2e5b1951fb8) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `PHP 8.4+ not installed in container; no system PHP available`
- 10 min: `sodium PHP extension missing in containerbase PHP build`
- 1 min: `zip binary not installed (archive:zip-binary test fails)`
- 5 min: `ssh/scp not installed (SSH tests fail)`
- `WaitForDockerTest requires Docker daemon , not available in container`
- `Notify* tests fail: no desktop notification system in headless container`
- `CommandBuilderLsTest: ls output ordering differs from expected ('.' in different position)`
- `EventListenerProcessTest: event ordering differs , 'Hello after process start' appears after 'Hello from process' instead of before`
- `RemoteImportRemoteTasksTest requires network access to external packages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
