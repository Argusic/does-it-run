# mac-cleaner-cli

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/guhcostan/mac-cleaner-cli, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mac-cleaner-cli

## Pinned environment

- Project commit: `9bc7c61b641893980fbdc277207ed7fbef076f0f`
- Test commit: `9bc7c61b641893980fbdc277207ed7fbef076f0f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.1 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 6.1 | 6 | 6 | [run](https://argusic.com/run/d805e583-7e01-4e95-9e5c-fb01b0f93695) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm 9.2.0 resolver bug: Cannot read properties of null (reading 'edgesOut')`
- 1 min: `Node v18.19.1 below required >=20.12.0 and project is os=darwin only`
- 1 min: `rolldown native binding missing for linux-x64-gnu (wasm32-wasi fallback fails)`
- 1 min: `Node 20 styleText API doesn't accept array of style names (needed Node 22+)`
- 0.5 min: `@inquirer/core not found at runtime (transitive dep not linked into pnpm store root by default)`
- 0.5 min: `Test execSync calls 'bun src/index.ts' but bun unavailable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
