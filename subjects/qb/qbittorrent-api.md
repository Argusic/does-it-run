# qbittorrent-api

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rmartin16/qbittorrent-api, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/qbittorrent-api

## Pinned environment

- Project commit: `13fcfb9a6867f3889c180e173f7be1b2806de747`
- Test commit: `13fcfb9a6867f3889c180e173f7be1b2806de747`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 14.4 to 14.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 14.4 | 3 | 3 | [run](https://argusic.com/run/31a0f395-35e9-4913-bc52-b143ae7941a5) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `conftest.py asserts BASE_PATH ends in 'qbittorrent-api' but the repo is at /work/repo`
- 0.1 min: `setup_environ() tries to contact a running qBittorrent during conftest import, which fails without one`
- 0.2 min: `no_state_left_behind fixture eagerly requests the client fixture even for offline tests, triggering session setup that requires a live qBittorrent`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
