# better-agents

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/langwatch/better-agents, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/better-agents

## Pinned environment

- Project commit: `00c44b92fafc245fa051a34910128e36e85aad07`
- Test commit: `00c44b92fafc245fa051a34910128e36e85aad07`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.4 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5.4 | 3 | 3 | [run](https://argusic.com/run/81e3e8a0-0bec-4f77-a2e5-4833911741b4) |
| 2 | pass | 100 | 7 | 6.4 | 1 | 1 | [run](https://argusic.com/run/c3ece3e2-2c0d-4da4-877c-f1593f2a9c4f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found in PATH (required by packageManager field)`
- 1 min: `Node v18.19.1 too old for rolldown native binding (requires ^20.19.0 || >=22.12.0)`
- 1 min: `@rolldown/binding-linux-x64-gnu optional dependency not installed by pnpm`

Attempt 2:

- 4 min: `pnpm build failed: tsdown → rolldown@1.0.0-beta.53 requires node:util:styleText (Node.js 22+) but container has Node 18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
