# edict

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cft0808/edict, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/edict

## Pinned environment

- Project commit: `14a207557719c046af0f993a7bff1cc5a5015b33`
- Test commit: `14a207557719c046af0f993a7bff1cc5a5015b33`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 6 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 2.5 | 6.1 | 3 | 3 | [run](https://argusic.com/run/6387ec75-ef2e-43cb-b952-ae1625e5c6d8) |
| 2 | pass | 100 | 8 | 6 | 3 | 3 | [run](https://argusic.com/run/5aa7410a-7b7f-420f-9b07-7d1143546873) |

## What was observed on a clean machine

Attempt 1:

- `OpenClaw CLI not installed; install.sh requires it`
- 2 min: `test_e2e_kanban: cmd_done transitions to Review not Done; test assertions out of sync with state machine`
- 2 min: `test_sync_symlinks: OPENCLAW_HOME imported at module level, not reachable by monkeypatch of pathlib.Path.home()`

Attempt 2:

- 1 min: `Broken symlinks for agentrec_advisor.py and linucb_router.py pointing to developer's local machine`
- 2 min: `test_sync_symlinks fixture didn't patch OPENCLAW_HOME which is evaluated at import time`
- 2 min: `test_done/test_done_not_overwritable used invalid state transitions (Zhongshu -> Done via cmd_done)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
