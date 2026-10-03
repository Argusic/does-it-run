# context7

**Verdict: runs with mocks.** Argusic Score 87.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/upstash/context7, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/context7

## Pinned environment

- Project commit: `6d777619c2777a79ad0754dc48b48845cb912bac`
- Test commit: `6d777619c2777a79ad0754dc48b48845cb912bac`
- Worker image digests: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`, `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 3; wall time 9.7 to 42 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 83.43 | 10 | 10.4 | 7 | 4 | [run](https://argusic.com/run/e67bbea5-02da-43d9-9650-033ebf8f959a) |
| 2 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/01ae8cc5-93bc-40cb-ba7e-e73e59feaf05) |
| 3 | pass with mocks | 92 | 6 | 9.7 | 5 | 5 | [run](https://argusic.com/run/da0a5a3f-0423-4e79-8999-eaf5ffd67f69) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed in container`
- 1 min: `Build scripts blocked by pnpm supply-chain policy`
- 2 min: `SDK client had hardcoded base URL preventing mock server use`
- 1 min: `Pi package had hardcoded base URL preventing mock server use`
- `3 CLI test suites fail: vitest v4 uses import attributes (with) unsupported in Node 18`
- `2 MCP test suites fail: undici v7 requires Node 20+ for global File constructor`
- `5 tools-ai-sdk tests fail: need AWS Bedrock credentials for real LLM calls`

Attempt 3:

- 1 min: `Node.js v18 lacked features required by dependencies (styleText, undici File, 'v' regex flag)`
- 1 min: `pnpm not installed`
- `pnpm-workspace.yaml had string placeholders instead of booleans for allowBuilds`
- 2 min: `SDK tests required CONTEXT7_API_KEY and hit live API`
- `5 tools-ai-sdk tests need AWS Bedrock credentials (AWS_REGION)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
