# sre

**Verdict: runs with mocks.** Argusic Score 86.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SmythOS/sre, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/sre

## Pinned environment

- Project commit: `5c382a1ec07accc75947c3e4fa24841532ae7c88`
- Test commit: `5c382a1ec07accc75947c3e4fa24841532ae7c88`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 27 to 27 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 86.29 | 2 | 27 | 7 | 5 | [run](https://argusic.com/run/4fbfc94b-b41e-4a78-bd4d-690e4efdef80) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `node:sqlite built-in module not found (Node.js 18 lacks it)`
- 0.5 min: `No vault file found at startup; SRE interactive prompt blocks tests`
- 1 min: `11 component test files expected no _debug field but agent mock set debug:true`
- 2 min: `Milvus mock client missing describeCollection method; search return lacked error_code`
- 1 min: `Scheduler LocalScheduler uses static jobs Map that leaks between tests`
- `17 AWS SecretsManager tests fail without real AWS credentials`
- `12 SDK/Core tests fail without real OPENAI_API_KEY`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
