# keycloak-config-cli

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/adorsys/keycloak-config-cli, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/keycloak-config-cli

## Pinned environment

- Project commit: `9c507e9acabe6b23f1d5faadd792ede875bd671b`
- Test commit: `9c507e9acabe6b23f1d5faadd792ede875bd671b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.4 to 4.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 4.4 | 2 | 2 | [run](https://argusic.com/run/5f54c4a3-d985-4ea5-aa33-a14fdf634f86) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `No Java runtime pre-installed`
- `Integration tests skipped: Docker not available (Testcontainers requires Docker)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
