# fastapi-observability

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/blueswen/fastapi-observability, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/fastapi-observability

## Pinned environment

- Project commit: `2764dba3e8b9f2ad692eb5377db988414201940d`
- Test commit: `2764dba3e8b9f2ad692eb5377db988414201940d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4 to 4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 4 | 4 | 4 | [run](https://argusic.com/run/06914cb6-a3f9-4a89-8c9e-d688f7716f3f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PEP 668 externally-managed-environment blocked system-wide pip install of project dependencies`
- 1 min: `uv (the documented package manager) is not installed in the container`
- 2 min: `siege (used by request-script.sh) is not installed and system packages cannot be installed without root`
- 2 min: `Docker is not available so the docker-compose full observability stack (Grafana/Prometheus/Tempo/Loki) cannot be stood up`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
