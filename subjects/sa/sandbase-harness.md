# sandbase-harness

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sandbaseai/sandbase-harness, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/sandbase-harness

## Pinned environment

- Project commit: `9fca646e8857d79b55671fb737d6492de7ddfd79`
- Test commit: `9fca646e8857d79b55671fb737d6492de7ddfd79`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 40.6 to 40.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 20 | 40.6 | 3 | 3 | [run](https://argusic.com/run/998e7ba3-882c-40b8-b1e9-f5afa27ec1cf) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `System Node 18.19.1/npm 9 are below the project's Node 22+/npm 10+ requirement; Node 22 tools failed with ERR_UNKNOWN_BUILTIN_MODULE node:sqlite`
- 5 min: `Background server processes died when the exec shell exited`
- 35 min: `First chat turns ended with no model output and span stop_reason 'other'; the mock got no requests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
