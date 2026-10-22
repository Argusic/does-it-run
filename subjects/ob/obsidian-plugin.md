# obsidian-plugin

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tldraw/obsidian-plugin, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/obsidian-plugin

## Pinned environment

- Project commit: `2a3b92638095128655ce786eeb717dc346a4d2d0`
- Test commit: `2a3b92638095128655ce786eeb717dc346a4d2d0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.8 to 3.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3.8 | 1 | 1 | [run](https://argusic.com/run/2220cf20-59cf-4e49-a2fa-f5699b849542) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `build script uses import.meta.dirname which is undefined on Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
