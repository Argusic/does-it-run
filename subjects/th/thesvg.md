# thesvg

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/glincker/thesvg, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/thesvg

## Pinned environment

- Project commit: `fa87032438a21826df5a4fbb0e6b0ce9d02147d6`
- Test commit: `fa87032438a21826df5a4fbb0e6b0ce9d02147d6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.1 to 3.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 12 | 3.1 | 4 | 3 | [run](https://argusic.com/run/a5b7f4a5-dc31-4dc3-8965-4ae187a7f404) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm lockfile supply-chain policy violation due to stale lockfile`
- 3 min: `Node 18.19 too old for rolldown/vitest (needs node:util styleText)`
- 1 min: `Missing @rolldown/binding-linux-x64-gnu native binding (optional dep not pulled by pnpm)`
- `pnpm.overrides in package.json ignored by pnpm 12 (non-fatal warning)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
