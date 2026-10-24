# list-sync

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Woahai321/list-sync, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/list-sync

## Pinned environment

- Project commit: `b635a833e1bb59ea51a2817bbc6d54b40ab97666`
- Test commit: `b635a833e1bb59ea51a2817bbc6d54b40ab97666`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.3 to 11.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 11.3 | 5 | 5 | [run](https://argusic.com/run/3907296a-8bf8-4bdd-b5fd-c0ffab02480f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Docker not available in container`
- 1 min: `System pip blocked by externally-managed-environment (PEP 668)`
- 2 min: `Node v18.19 too old for Nuxt 3.17 (needs ^20.19.0 || ^22.12.0 || >=23)`
- 2 min: `Chrome/Chromium not installed - Selenium init fails in core sync engine`
- 1 min: `Dependency version conflicts: requests 2.34.2->2.31.0, psutil 7.2.2->5.9.6 due to api_requirements.txt pins`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
