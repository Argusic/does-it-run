# bux

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/browser-use/bux, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/bux

## Pinned environment

- Project commit: `f17c1b31d6688dd92e745ade650e00d46b4dc4da`
- Test commit: `f17c1b31d6688dd92e745ade650e00d46b4dc4da`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3.9 to 3.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.05 | 3.9 | 1 | 1 | [run](https://argusic.com/run/465b369a-33cf-46d1-8dfb-d84c3a020838) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_login_flow.py::test_forced_claude_login_restarts_existing_shell failed: save_state tries to write to /etc/bux/tg-state.tmp which doesn't exist in the container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
