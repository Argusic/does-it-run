# event-management

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PuneethReddyHC/event-management, licensed Apache-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/event-management

## Pinned environment

- Project commit: `478d48309b64ddab54aeee59581cf90d1231953f`
- Test commit: `478d48309b64ddab54aeee59581cf90d1231953f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.7 to 24.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 24.7 | 5 | 5 | [run](https://argusic.com/run/e1000325-9d49-4606-bd89-90580ed23c94) |

## What was observed on a clean machine

Attempt 1:

- 18 min: `No PHP or MySQL installed in container`
- 5 min: `MariaDB initialization failed: --initialize and --initialize-insecure options not supported in MariaDB 10.11`
- 7 min: `FrankenPHP PHP CLI has seccomp sandbox (level 2) blocking network connections`
- 1 min: `session_start(): Session cannot be started after headers have already been sent in index.php`
- 4 min: `MariaDB server kept crashing in background mode due to stale PID files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
