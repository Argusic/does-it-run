# Tianshu-harness

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/huiliyi37/Tianshu-harness, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tianshu-harness

## Pinned environment

- Project commit: `0f034d4379db29834b0e471ffe59d7888fcbdb90`
- Test commit: `0f034d4379db29834b0e471ffe59d7888fcbdb90`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 19 to 19 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 20 | 19 | 3 | 3 | [run](https://argusic.com/run/26316b87-a0e3-4232-8911-2075700eb4ff) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node v18.19.1 too old; project requires Node >=24 (engine-strict)`
- 6 min: `Headless run failed 'Cannot read properties of undefined (reading id)': registering provider with --api-key-env created a provider-keys.json key pool with no models, and contractModels reads that key pool (not top-level models) so model poo`
- 4 min: `Mock returned plain JSON completion; app correctly rejected 'content-type is application/json (not SSE stream)'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
