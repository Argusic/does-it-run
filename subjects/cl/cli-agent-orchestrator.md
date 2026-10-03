# cli-agent-orchestrator

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/awslabs/cli-agent-orchestrator, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/cli-agent-orchestrator

## Pinned environment

- Project commit: `dc5efb3179742bed5bca7f0c17f2a4b5d52a9f4c`
- Test commit: `dc5efb3179742bed5bca7f0c17f2a4b5d52a9f4c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 42.8 to 98.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 89 | 98.3 | 4 | 4 | [run](https://argusic.com/run/969aa512-d2ef-4fb9-b34e-d4d27d9f8d2b) |
| 2 | pass | 96 | 5 | 42.8 | 5 | 4 | [run](https://argusic.com/run/7b9c9191-7856-4c53-95f9-9fa85783e012) |

## What was observed on a clean machine

Attempt 1:

- 45 min: `tmux >=3.3 not available (no root to apt-get install); prebuilt binaries incompatible (GLIBC 2.42, ncurses 6.5); source build linked 145 .o files but ld hung on final link step`
- 2 min: `ag-ui-protocol optional dependency not installed by default, causing 18 test failures`
- `4 test_wiki_lint.py ContradictionRetraction tests fail without a real LLM`
- `3 test_session_service.py tests fail because they need a running tmux to create worker terminals`

Attempt 2:

- 2 min: `tmux not on PATH`
- 1 min: `uv not installed`
- 1 min: `ag-ui-protocol missing (optional dep [agui])`
- 1 min: `Node.js 18.19 too old for Vite (needs 20.19+)`
- 1 min: `4 wiki_lint test failures (test-isolation bugs, not env)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
