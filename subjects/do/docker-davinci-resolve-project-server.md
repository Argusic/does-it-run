# Docker-Davinci-Resolve-Project-Server

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elliotmatson/Docker-Davinci-Resolve-Project-Server, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/docker-davinci-resolve-project-server

## Pinned environment

- Project commit: `3855ab46264cd03447f1d34e134714768a702423`
- Test commit: `3855ab46264cd03447f1d34e134714768a702423`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.6 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 4.6 | 2 | 2 | [run](https://argusic.com/run/a067b610-37db-4e5f-89ee-5280fca24167) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Docker not available in container (no root). Extracted PostgreSQL 16 from apt .deb packages instead of using compose image postgres:13.`
- 1 min: `PostgreSQL couldn't create lock file at /var/run/postgresql (permission denied).`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
