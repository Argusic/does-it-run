# home-assistant-config

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/basnijholt/home-assistant-config, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/home-assistant-config

## Pinned environment

- Project commit: `3b7b439761c4be7b854278b6e6d094a668712595`
- Test commit: `3b7b439761c4be7b854278b6e6d094a668712595`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.8 to 17.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 17.8 | 8 | 8 | [run](https://argusic.com/run/328d440f-d7a4-4c39-84e2-76bc5367aa5b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing secrets.yaml with dummy values`
- 2 min: `Broken symlink custom_components/adaptive_lighting`
- 1 min: `Missing custom_components/pyscript`
- 5 min: `Python C headers (Python.h) not found, blocking netifaces build`
- 1 min: `allowlist_external_dirs pointed to non-existent /config/`
- 1 min: `db_url pointed to non-writable /config/home-assistant.db`
- 2 min: `aiodiscover/aiodns version conflict with HA requirements`
- 3 min: `pyspeex-noise==1.0.2 fails to build (no root for python3-dev)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
