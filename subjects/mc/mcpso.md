# mcpso

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chatmcp/mcpso, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mcpso

## Pinned environment

- Project commit: `e14f33850f449dce186eb78bbf05b075065c2ca4`
- Test commit: `e14f33850f449dce186eb78bbf05b075065c2ca4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 6.3 to 9.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 6.3 | 3 | 3 | [run](https://argusic.com/run/940cda0c-06df-4a8c-beec-1fb1b5a60df0) |
| 2 | fail | 20 | n/a | 9.2 | 0 | 0 | [run](https://argusic.com/run/00a844c1-5b63-4f48-954f-487b8b427fa3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found in environment`
- 2 min: `ERR_PNPM_IGNORED_BUILDS: esbuild, sharp, workder builds blocked`
- 1 min: `TypeScript error: KeyboardEvent<HTMLInputElement> is not generic when using @types/react@18 with React 19`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
