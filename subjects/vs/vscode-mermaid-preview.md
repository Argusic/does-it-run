# vscode-mermaid-preview

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Mermaid-Chart/vscode-mermaid-preview, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vscode-mermaid-preview

## Pinned environment

- Project commit: `6e98ec94ffe06be6ef4c00339a2d8e7da6546e0c`
- Test commit: `6e98ec94ffe06be6ef4c00339a2d8e7da6546e0c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 19.2 to 19.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 19 | 19.2 | 5 | 5 | [run](https://argusic.com/run/192f05a6-b834-4131-a182-f3b08a7ac3e0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pnpm not installed and no root for global npm install`
- 8 min: `pnpm install 401: 5 private @mermaid-chart/* packages hosted on GitHub Packages require auth`
- 2 min: `TypeScript 4.9.5 cannot parse modern @types/d3-dispatch@3.0.7 (const type parameters) pulled by public mermaid`
- 5 min: `pnpm test failed: out/test/runTest.js never emitted (compile uses tsc --noEmit; rootDir . emits to out/src/test)`
- 2 min: `pnpm package crashed: undici@7.30.1 requires Node >=20.18.1 (File is not defined on Node 18.19.1)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
