# photoshop-mcp

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alisaitteke/photoshop-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/photoshop-mcp

## Pinned environment

- Project commit: `a0b73188ba77feba331ff5bfe73934aca5bef957`
- Test commit: `a0b73188ba77feba331ff5bfe73934aca5bef957`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 4.7 to 34.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 34.5 | 4 | 4 | [run](https://argusic.com/run/821749db-a2ba-4abb-a6c0-46ae72f3bda8) |
| 2 | pass | 100 | 4.5 | 4.7 | 1 | 1 | [run](https://argusic.com/run/0cc220bb-7fc4-4185-91f3-5c4c553c3f6c) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `npm install failed: @tailwindcss/oxide native binding missing (npm #4828 optional-deps bug)`
- 3 min: `vitest 4 cannot start on Node 18.19.1 (node:util.styleText missing)`
- 15 min: `better-sqlite3 v12 prebuilt binary linked to libnode.so.109 ABI 109 segfaults under Node 20 (ABI 115), crashing 5 suite files`
- 8 min: `npm runtime mismatch: CLI/test scripts spawn 'npx' which resolves Node 18 under this PATH, but Node 20 crashes sqlite paths`

Attempt 2:

- 3 min: `Web UI frontend build failed: @tailwindcss/oxide native binding requires Node 20+ but container has Node 18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
