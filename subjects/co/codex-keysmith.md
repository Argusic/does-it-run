# codex-keysmith

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Jia-Ethan/codex-keysmith, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/codex-keysmith

## Pinned environment

- Project commit: `c4d3f48067889f40932f93c03303285447c00dda`
- Test commit: `c4d3f48067889f40932f93c03303285447c00dda`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.8 to 10.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 9 | 10.8 | 1 | 0 | [run](https://argusic.com/run/3f793ef0-b61d-4b44-8798-c7aca8f1c710) |
| 2 | pass | 100 | 2 | 6.8 | 2 | 2 | [run](https://argusic.com/run/561d1e03-1e94-4976-ac3a-8cd54525adf6) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `GUI npm test fails: @tailwindcss/oxide native binary missing for linux-x64-gnu , cannot build/test the Tauri/React frontend`

Attempt 2:

- 1 min: `pip install --user blocked by PEP 668 externally-managed-environment`
- 1 min: `gui npm test failed: MODULE_NOT_FOUND @tailwindcss/oxide/tailwindcss-oxide.linux-x64-gnu.node (npm 9 skipped the platform optional dep on this musl libc host)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
