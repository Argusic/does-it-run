# app-ssh

**Verdict: could not verify.** Argusic Score 30 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hassio-addons/app-ssh, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/app-ssh

## Pinned environment

- Project commit: `60a2d61b7ef15eb9c3c7fa790e24536d23f32af6`
- Test commit: `60a2d61b7ef15eb9c3c7fa790e24536d23f32af6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 5.1 to 6.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 30 | 0 | 5.1 | 3 | 0 | [run](https://argusic.com/run/84c75bc8-467a-4af0-bded-df32e6b91da4) |
| 2 | fail | 30 | 40 | 6.9 | 3 | 0 | [run](https://argusic.com/run/2a7cd995-0a4d-486f-93da-6311bdc95468) |

## What was observed on a clean machine

Attempt 1:

- `Docker is not available in this container environment , no daemon socket, no root access to install it, and the user is non-root.`
- `Cannot install system packages (apk/apt) , no root privileges in this container.`
- `Cannot run the app or execute the Dockerfile build , this is a Home Assistant Supervisor addon that runs inside a specific HA environment, not a standalone application.`

Attempt 2:

- `Docker not available in container - cannot build the Docker image for this HA add-on`
- `No test suite exists in the repository - CI is an external reusable workflow`
- `Cannot run sshd/ttyd stack without HA Supervisor environment (bashio, s6-overlay, SUPERVISOR_TOKEN)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
