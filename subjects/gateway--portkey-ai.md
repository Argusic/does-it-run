# gateway

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Portkey-AI/gateway, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/f0da9163-d88c-4c55-a093-60c5c9ab9036

## Pinned environment

- Project commit: `669825cbe89ee51569918b8f78a9db486fd69dd4`
- Test commit: `669825cbe89ee51569918b8f78a9db486fd69dd4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 30.2 to 30.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 30.2 | 7 | 7 | [run](https://argusic.com/run/f0da9163-d88c-4c55-a093-60c5c9ab9036) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `jest.mock() paths in 4 test files pointed into tests/ instead of src/`
- 5 min: `ResponseService constructor signature drift: test passed 4 args but source expects 2 (RequestContext, HooksService)`
- 2 min: `PreRequestValidatorService.getResponse() return type changed; tests accessed .status on wrapper object`
- 3 min: `ProviderContext.getHeaders/getBaseURL mock expectations mismatched source API`
- 5 min: `Top-level await in src/utils/env.ts incompatible with ts-jest CommonJS transform`
- 1 min: `TypeScript error: 'version' missing from Params interface (src/types/requestBody.ts)`
- 1 min: `TypeScript error: 'default' property on union type ParameterConfig | ParameterConfig[] (src/providers/open-ai-base/index.ts)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
