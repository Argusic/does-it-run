# jampack

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/divriots/jampack, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/jampack

## Pinned environment

- Project commit: `6b5410035f96b3f2bd34ba6067f68c6d461fa5a6`
- Test commit: `6b5410035f96b3f2bd34ba6067f68c6d461fa5a6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 2.5 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 2 | 2.5 | 3 | 3 | [run](https://argusic.com/run/c71096fb-dfcb-487d-a998-73f060b3d18e) |
| 2 | pass | 100 | 3 | 3.2 | 5 | 5 | [run](https://argusic.com/run/2bb37431-45d5-41da-9dd8-2bf25b34264d) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pnpm not found in PATH`
- 0.5 min: `pnpm install blocked by unapproved build scripts for @swc/core, esbuild, sharp`
- 0.5 min: `@swc/core native binding failed: cache root /home/runner/.cache has wrong permissions (no sticky bit)`

Attempt 2:

- 1 min: `pnpm not available in PATH`
- 0.1 min: `pnpm lockfile version 6.0 incompatible with pnpm 12.x`
- 0.5 min: `pnpm ignored build scripts for @swc/core, esbuild, sharp`
- 0.5 min: `@swc/core native binding failed due to /home/runner/.cache permissions`
- `npm install failed with 'Cannot read properties of null (reading matches)'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
