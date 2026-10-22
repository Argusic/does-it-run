# photoshop-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alisaitteke/photoshop-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/photoshop-mcp

## Pinned environment

- Project commit: `a0b73188ba77feba331ff5bfe73934aca5bef957`
- Test commit: `a0b73188ba77feba331ff5bfe73934aca5bef957`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 34.5 to 34.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 34.5 | 4 | 4 | [run](https://argusic.com/run/821749db-a2ba-4abb-a6c0-46ae72f3bda8) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `npm install failed: @tailwindcss/oxide native binding missing (npm #4828 optional-deps bug)`
- 3 min: `vitest 4 cannot start on Node 18.19.1 (node:util.styleText missing)`
- 15 min: `better-sqlite3 v12 prebuilt binary linked to libnode.so.109 ABI 109 segfaults under Node 20 (ABI 115), crashing 5 suite files`
- 8 min: `npm runtime mismatch: CLI/test scripts spawn 'npx' which resolves Node 18 under this PATH, but Node 20 crashes sqlite paths`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
