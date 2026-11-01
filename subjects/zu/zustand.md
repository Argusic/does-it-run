# zustand

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pmndrs/zustand, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/zustand

## Pinned environment

- Project commit: `d7a5583cffd80af515f7dfb69583c95cbdc9e2ce`
- Test commit: `d7a5583cffd80af515f7dfb69583c95cbdc9e2ce`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.3 to 23.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 23.7 | 1 | 1 | [run](https://argusic.com/run/d1224b81-4a40-4a4a-88a0-7a655fe1bb9e) |
| 2 | pass | 100 | 5 | 5.3 | 4 | 4 | [run](https://argusic.com/run/2d7be91d-ded3-4497-815b-2741d5c612d0) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `jsdom@30 requires Node >=22, container has Node 18.19.1; also @exodus/bytes is ESM-only but html-encoding-sniffer/whatwg-url/jsdom all require() it`

Attempt 2:

- 1 min: `pnpm-workspace.yaml missing 'packages' field`
- 1 min: `Vitest 4.x incompatible with Node 18.19`
- 1 min: `jsdom 30.x requires ESM-only dep not supported by vitest 2's CJS worker`
- 1 min: `toHaveBeenCalledExactlyOnceWith not available in vitest 2.x matchers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
