# premiere-pro-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/leancoderkavy/premiere-pro-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/premiere-pro-mcp

## Pinned environment

- Project commit: `c2a91a33e6696a46623e8975fb0a5b8573e827a9`
- Test commit: `c2a91a33e6696a46623e8975fb0a5b8573e827a9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3.9 to 3.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 3.9 | 1 | 1 | [run](https://argusic.com/run/78d9ce66-76a5-4478-8f0f-3fa8bd2c4393) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18.19.1 installed but project requires ^20.20.0 || >=22.22.0 , vitest/rolldown fail at runtime with SyntaxError: missing styleText export`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
