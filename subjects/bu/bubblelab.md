# BubbleLab

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bubblelabai/BubbleLab, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/bubblelab

## Pinned environment

- Project commit: `e64b2469659b72156ca02a767e38cf73913c40d7`
- Test commit: `e64b2469659b72156ca02a767e38cf73913c40d7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 27 to 45.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 27 | 5 | 5 | [run](https://argusic.com/run/b38d94e8-4e9d-4f69-8b9d-88e00197a49a) |
| 2 | pass | 100 | 45 | 45.9 | 5 | 5 | [run](https://argusic.com/run/60702222-7e10-4ddb-bde6-ac4a6746794e) |

## What was observed on a clean machine

Attempt 1:

- `Node.js v18.19.1 installed but project requires >=20; pnpm install warns`
- 0.5 min: `pnpm not found initially; npm install -g failed (no root)`
- 1 min: `bun not found; npm install -g failed (no root); unzip not available`
- 0.5 min: `pnpm blocked build scripts for esbuild, protobufjs, core-js, @clerk/shared, @tailwindcss/oxide`
- `bubble-studio tests exit 1 due to jsdom/webidl-conversions TypeError on Node 18`

Attempt 2:

- 2 min: `Node.js v18 is too old, project requires >=20`
- 1 min: `pnpm not found in PATH`
- 2 min: `bun not found (required by bubblelab-api)`
- `SQLITE_BUSY errors when running full test suite due to concurrent test files`
- `boba.test.ts AI generation test fails with real OPENROUTER_API_KEY - generated code doesn't pass TypeScript validation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
