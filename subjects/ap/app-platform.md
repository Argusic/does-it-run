# app-platform

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ModelEngine-Group/app-platform, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/app-platform

## Pinned environment

- Project commit: `dd242b21cb136c871b1658b9594616a29a2f8246`
- Test commit: `dd242b21cb136c871b1658b9594616a29a2f8246`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 64.9 to 64.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 64 | 64.9 | 5 | 5 | [run](https://argusic.com/run/9adec033-afed-42fb-881c-8b12270aba02) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Java JDK 17 not pre-installed in container`
- 1 min: `Maven not pre-installed in container`
- 0.1 min: `Frontend npm install failed due to @types/react-dom@16 peer dep incompatible with React 18 types`
- 0.3 min: `Frontend dev server (webpack serve) failed due to missing react-refresh peer dependency`
- `Docker and docker-compose not available in container, blocking docker/deploy.sh deployment path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
