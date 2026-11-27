# m3e-canvas

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lnkiai/m3e-canvas, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/m3e-canvas

## Pinned environment

- Project commit: `de2d97a577b2b77f33428db11c658e3548335b5e`
- Test commit: `de2d97a577b2b77f33428db11c658e3548335b5e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.7 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 7.7 | 3 | 3 | [run](https://argusic.com/run/d7de60dd-4af5-4075-a011-c95dcd2aa207) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 is below the required >=20.9.0 for Next.js 16 and the project's engines (^22.12.0).`
- 2 min: `@tailwindcss/oxide native binding 'tailwindcss-oxide.linux-x64-gnu.node' missing , npm's optional dependency resolution failed to install the platform-specific package into the expected location.`
- 1 min: `Existing '.npmrc' with 'prefix=/home/runner/npm-global' caused repeated warnings and interfered with npm.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
