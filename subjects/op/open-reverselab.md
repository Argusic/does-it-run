# open-reverselab

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LING71671/open-reverselab, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/open-reverselab

## Pinned environment

- Project commit: `19018aeea7a165f75b483decd6991433f5a086ae`
- Test commit: `19018aeea7a165f75b483decd6991433f5a086ae`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.8 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 1.8 | 3 | 3 | [run](https://argusic.com/run/a23d1372-08e0-4705-8707-28649e88f232) |
| 2 | pass | 100 | 4 | 2.2 | 4 | 4 | [run](https://argusic.com/run/f277cc87-4a17-4c1d-a940-78b53ebd5093) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install blocked by externally-managed-environment`
- 1 min: `MCP smoke check failed: 'uv' not found in PATH`
- `Missing optional external tools (Java, Go, Docker, sqlmap, mitmproxy, etc.)`

Attempt 2:

- 0.5 min: `uv not installed system-wide (externally-managed Python environment)`
- 0.5 min: `pnpm not available globally (EACCES)`
- `Desktop JS tests: 8/12 failed , Node v18 lacks crypto global, styleText, JSON with imports support`
- `tailwindcss/vite requires Node >=20 , desktop vite build may fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
