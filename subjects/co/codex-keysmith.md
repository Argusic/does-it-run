# codex-keysmith

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Jia-Ethan/codex-keysmith, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/codex-keysmith

## Pinned environment

- Project commit: `c4d3f48067889f40932f93c03303285447c00dda`
- Test commit: `c4d3f48067889f40932f93c03303285447c00dda`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.8 to 10.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 9 | 10.8 | 1 | 0 | [run](https://argusic.com/run/3f793ef0-b61d-4b44-8798-c7aca8f1c710) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `GUI npm test fails: @tailwindcss/oxide native binary missing for linux-x64-gnu , cannot build/test the Tauri/React frontend`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
