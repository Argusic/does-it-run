# sno-station

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sno-ai/sno-station, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/sno-station

## Pinned environment

- Project commit: `bbb01afeb56ac6058b426c56640885028979aae3`
- Test commit: `bbb01afeb56ac6058b426c56640885028979aae3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 15.1 to 15.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 28 | 15.1 | 6 | 6 | [run](https://argusic.com/run/98441262-1814-4b76-b289-5385f7023247) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `System Node.js v18.19.1 is too old (requires >=24.15.0)`
- 3 min: `openclaw preinstall script hard-blocks Node <22.22.3`
- 2 min: `onnxruntime-node install script fails with 404 on CUDA binary download`
- 2 min: `tsdown (rolldown/code bundler) requires Node 22+`
- 1 min: `vitest 4.x requires Node 22+`
- 5 min: `10 mem-claw unit test files fail (26/90 tests) with sidecar-unreachable and crypto init errors`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
