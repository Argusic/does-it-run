# ironcurtain

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/provos/ironcurtain, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ironcurtain

## Pinned environment

- Project commit: `8f9c75a720337271caf1e18c199fcca2d299ad27`
- Test commit: `8f9c75a720337271caf1e18c199fcca2d299ad27`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.7 to 16.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 16 | 16.7 | 4 | 2 | [run](https://argusic.com/run/a195b3aa-5cb9-4aa6-9bb4-0405cd4328ff) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js 18 installed but project requires Node 24+`
- 1 min: `npm install-scripts for native modules (isolated-vm, node-pty, esbuild) not automatically run by npm`
- `test/mux-input-handler.test.ts: 1 pre-existing test failure - handlePaste returns 'redraw-picker' when list-focused with no entries, test expects 'none'`
- `test/workflow/nested-docker-live-smoke.test.ts: 1 pre-existing test failure - needs Docker daemon (unavailable in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
