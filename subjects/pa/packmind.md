# packmind

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PackmindHub/packmind, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/packmind

## Pinned environment

- Project commit: `ded906d148591dc534399aac4605bc3e1936c79e`
- Test commit: `ded906d148591dc534399aac4605bc3e1936c79e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.9 to 9.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 9.9 | 3 | 3 | [run](https://argusic.com/run/32d9121a-c7b9-4158-a0b4-08f2fd2a043a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node v18 detected but project requires >=24.13.0. pnpm not found.`
- 1 min: `Missing tsconfig.base.effective.json referenced by all tsconfig files`
- 3 min: `CLI dist binary failed with 'Cannot find module minimatch'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
