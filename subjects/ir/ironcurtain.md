# ironcurtain

**Verdict: runs.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/provos/ironcurtain, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ironcurtain

## Pinned environment

- Project commit: `8f9c75a720337271caf1e18c199fcca2d299ad27`
- Test commit: `8f9c75a720337271caf1e18c199fcca2d299ad27`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 16.7 to 24.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 16 | 16.7 | 4 | 2 | [run](https://argusic.com/run/a195b3aa-5cb9-4aa6-9bb4-0405cd4328ff) |
| 2 | pass with mocks | 82 | 25 | 24.4 | 4 | 2 | [run](https://argusic.com/run/b19f370e-ab3b-45db-af05-5b1632a6612b) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js 18 installed but project requires Node 24+`
- 1 min: `npm install-scripts for native modules (isolated-vm, node-pty, esbuild) not automatically run by npm`
- `test/mux-input-handler.test.ts: 1 pre-existing test failure - handlePaste returns 'redraw-picker' when list-focused with no entries, test expects 'none'`
- `test/workflow/nested-docker-live-smoke.test.ts: 1 pre-existing test failure - needs Docker daemon (unavailable in container)`

Attempt 2:

- 8 min: `Node.js v18.19.1 in container is below project minimum (^24.0.0 || ^26.0.0); npm install required --ignore-scripts to skip native addon isolated-vm@7.0.1 which cannot compile on Node 18`
- 15 min: `vitest@4 and vite@8 (pulled in by packages/web-ui workspace) use rolldown which imports styleText from node:util (Node 20+) , vitest fails to start on Node 18`
- `Docker is not available in the container; tests requiring Docker (docker-manager, docker-infrastructure, etc.) are expected to fail`
- `33 of 194 test files failed (74 of 4052 individual tests) , primarily due to Node 18 lacking crypto.randomUUID in ESM fork context (uuid@14), File constructor (Node 20+), and import attributes syntax`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
