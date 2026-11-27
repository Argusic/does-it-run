# Claude-Cage

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Lee-xeo/Claude-Cage, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/claude-cage

## Pinned environment

- Project commit: `b598e2ee1c90145bd294bd9643f0196a6a96717f`
- Test commit: `b598e2ee1c90145bd294bd9643f0196a6a96717f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28.7 to 28.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17 | 28.7 | 6 | 6 | [run](https://argusic.com/run/90766e48-b9e2-424d-b4f5-18237c90361b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.26.10 not installed in container`
- 1 min: `Node.js v18 too old for Vite 8 (requires ^20.19.0)`
- 1 min: `uv tool missing (prepare-vnc.mjs requires 'uv run python')`
- 1 min: `UI web assets not built (internal/workbench/web/ empty)`
- 1 min: `/usr/bin/ssh not found (code hardcoded path)`
- `ssh-keygen not found (needed by vm tests)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
