# goatdb

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/goatplatform/goatdb, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/goatdb

## Pinned environment

- Project commit: `8fdf7373b9260cf3010996f7a49a93c73e4bb566`
- Test commit: `8fdf7373b9260cf3010996f7a49a93c73e4bb566`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.2 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 5.5 | 2 | 2 | [run](https://argusic.com/run/212da5cd-026d-4dbe-b5e5-0ab415e819cf) |
| 2 | pass | 100 | 4 | 4.2 | 4 | 4 | [run](https://argusic.com/run/35334fd6-89a4-4adf-89e4-4ff66b1b521d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Deno not installed`
- 1 min: `Node.js v18 too old (needs 24+)`

Attempt 2:

- 1 min: `Deno not found in system PATH`
- 0.5 min: `unzip not available for Deno install script`
- 1.5 min: `Node.js v18 had import syntax error bundling for Node tests`
- 0.5 min: `Playwright install --with-deps failed due to no root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
