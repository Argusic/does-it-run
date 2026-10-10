# libtmux

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tmux-python/libtmux, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/libtmux

## Pinned environment

- Project commit: `500f99b6cab442c6c6eaaa45275d455ac65ff732`
- Test commit: `500f99b6cab442c6c6eaaa45275d455ac65ff732`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.3 to 7.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 7.3 | 3 | 3 | [run](https://argusic.com/run/b2337803-8197-4a89-93c6-50d560be7aed) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `tmux binary not available in container (required by libtmux)`
- 1 min: `conftest.py references doctest_namespace fixture from pytest's doctest plugin, but project config disables doctest plugin via -p no:doctest, causing fixture resolution error`
- 1 min: `test_control_mode_stdout_preserves_non_ascii_output fails under LC_CTYPE=C (pre-existing locale bug with control-mode output of non-ASCII chars)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
