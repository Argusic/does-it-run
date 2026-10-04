# univer-workspace

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dream-num/univer-workspace, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/univer-workspace

## Pinned environment

- Project commit: `bf1286479998c07d81a5d396a437d57fc6a31a00`
- Test commit: `bf1286479998c07d81a5d396a437d57fc6a31a00`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.7 to 26.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 27 | 26.7 | 5 | 5 | [run](https://argusic.com/run/757d9716-db61-4915-9022-532e623d9903) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 in container, requires ≥24`
- 1 min: `pnpm not found`
- 2 min: `Corepack auto-selects pnpm 12.9.1 but its cached bin/ dir contains .mjs files while .corepack points to .cjs`
- 3 min: `apps/agent/desktop/src/dsh-host.cjs:64 uses context.conditions.includes() which fails with SafeSet (CJS resolve hook) , TypeError in host-resolution.test`
- 1 min: `pnpm test OOM-kills client-core due to parallel vitest fork workers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
