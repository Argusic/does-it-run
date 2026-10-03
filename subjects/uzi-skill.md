# UZI-Skill

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wbh604/UZI-Skill, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/uzi-skill

## Pinned environment

- Project commit: `650788c54a9b2e042bf7f983f16dbf8d727fce1d`
- Test commit: `650788c54a9b2e042bf7f983f16dbf8d727fce1d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 21.1 to 21.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 20 | 21.1 | 3 | 3 | [run](https://argusic.com/run/58e011f8-fd59-4adb-8400-7766d4212edf) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Debian externally-managed-environment blocks system-wide pip install`
- 0.5 min: `pytest not pre-installed in venv`
- 10 min: `Lite end-to-end run on 600519.SH timed out on 3/22 fetchers from overseas (4_peers, 12_capital_flow, similar_stocks)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
