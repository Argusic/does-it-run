# mcp_excalidraw

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yctimlin/mcp_excalidraw, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mcp-excalidraw

## Pinned environment

- Project commit: `713706e967ed21db1d9264748fa01c6af961c792`
- Test commit: `713706e967ed21db1d9264748fa01c6af961c792`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27.2 to 27.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 27.2 | 2 | 2 | [run](https://argusic.com/run/c98d4c3b-2986-494e-8089-066882f01d41) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js version 18 too old, required >=20`
- 10 min: `Frontend vite build OOM-killed during rendering chunks phase (needs >1.5GB RAM, only 2GB avail with no swap)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
