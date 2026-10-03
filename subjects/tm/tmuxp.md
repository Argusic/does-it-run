# tmuxp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tmux-python/tmuxp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/tmuxp

## Pinned environment

- Project commit: `31533713110555fc71fc0aa74b10cb9ec7591282`
- Test commit: `31533713110555fc71fc0aa74b10cb9ec7591282`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.6 to 10.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 10.6 | 8 | 8 | [run](https://argusic.com/run/90e4b4c3-2d88-4257-9166-f2351684454f) |

## What was observed on a clean machine

Attempt 1:

- `python not found (bare 'python' command)`
- 5 min: `tmux binary not installed`
- 2 min: `libutempter.so.0 missing for extracted tmux binary`
- 2 min: `libevent_core-2.1.so.7 missing for extracted tmux binary`
- 2 min: `pip install failed due to externally-managed-environment`
- 2 min: `tests/test_docs_tmux_layout.py ImportError: No module named docutils/sphinx`
- 1 min: `test_search_no_args_shows_help - tmuxp not on PATH for subprocess calls`
- 1 min: `test_highlight_matches_with_colors/test_highlight_matches_multiple fail due to NO_COLOR=1 env var`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
