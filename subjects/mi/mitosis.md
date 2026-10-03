# mitosis

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BuilderIO/mitosis, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mitosis

## Pinned environment

- Project commit: `cb1e2105c21971f336a1d8a4ff9a0406716471a0`
- Test commit: `cb1e2105c21971f336a1d8a4ff9a0406716471a0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 30.3 to 30.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 0.87 | 30.3 | 5 | 0 | [run](https://argusic.com/run/8073f39a-b46c-4a0e-a3a4-3e82afea388a) |

## What was observed on a clean machine

Attempt 1:

- `@builder.io/e2e-app-qwik build: TS2551 Property 'value' does not exist on type 'string[]' in generated signal-item-list.tsx`
- `@builder.io/e2e-angular build: TS2551 Property 'value' does not exist on type 'string[]' in generated signal-item-list.ts`
- `@builder.io/mitosis-fiddle build: Node.js OOM during Next.js SSR build`
- `@builder.io/mitosis-site build: Node.js OOM during Qwik SSR build`
- `core test: 32 snapshot mismatches (31x signalsOnUpdate, 1x findSignals)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
