# proxy_pool

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jhao104/proxy_pool, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/proxy-pool

## Pinned environment

- Project commit: `9cc0cad4c47e84e34aaec2eead099421960dcd07`
- Test commit: `9cc0cad4c47e84e34aaec2eead099421960dcd07`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 4.1 to 5.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.5 | 5.6 | 3 | 3 | [run](https://argusic.com/run/46617773-bcae-4fb4-9da7-f1948c03d207) |
| 2 | pass with mocks | 92 | 8 | 4.1 | 2 | 2 | [run](https://argusic.com/run/4e28856e-ed67-423f-8b0b-8e1b27c2b189) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `lxml==4.9.2 failed to build from source (missing libxml2-dev/libxslt-dev headers)`
- 0.5 min: `gunicorn==19.9.0 ModuleNotFoundError: No module named 'gunicorn.six.moves' on Python 3.12`
- 3 min: `no redis-server available and no root for apt install`

Attempt 2:

- 1 min: `externally-managed-environment blocks system pip`
- 2 min: `lxml==4.9.2 requires libxml2-dev headers to build from source`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
