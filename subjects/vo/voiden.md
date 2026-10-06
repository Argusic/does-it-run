# voiden

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/VoidenHQ/voiden, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/voiden

## Pinned environment

- Project commit: `e9ac33e2ead99aeebf2a6aff0c837656da04dcb7`
- Test commit: `e9ac33e2ead99aeebf2a6aff0c837656da04dcb7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.3 to 13.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 13.3 | 7 | 7 | [run](https://argusic.com/run/0372649d-5959-4840-91cb-b35fa823ba3e) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18.19.1 too old (requires v21+); Corepack not available with bundled Node`
- `yarn not installed in container`
- 1 min: `vite.config.ts root path doubled when building UI from workspace root`
- 2 min: `tailwind.config.js contained v2 'darkMode' and 'safelist' keys not valid in v3`
- 1 min: `postcss.config.js referenced './apps/ui/tailwind.config.js' (wrong relative path)`
- 1 min: `Electron test fails due to missing Electron runtime (window.ts references app.name)`
- 5 min: `UI build fails on tailwindcss v3 incompatibility (reading undefined 'blocklist')`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
