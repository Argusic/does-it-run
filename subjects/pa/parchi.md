# parchi

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/0xSero/parchi, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/parchi

## Pinned environment

- Project commit: `0678f72a3e16fdac7b4fdcda566dd6f4d91854b9`
- Test commit: `0678f72a3e16fdac7b4fdcda566dd6f4d91854b9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 11.7 to 19.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 19.6 | 0 | 0 | [run](https://argusic.com/run/942d38c2-a874-447c-90e6-12621fa38f10) |
| 2 | pass with mocks | 92 | 35 | 11.7 | 3 | 3 | [run](https://argusic.com/run/d4f8690d-4062-4523-9019-5187a2016c13) |

## What was observed on a clean machine

Attempt 2:

- `npm WARN EBADENGINE: 20+ packages require node >=20 but node v18.19.1 is installed`
- `npm test: 9/21 E2E tests timed out in headless virtual display (panel loading, quick actions, new session, theme, look-and-feel, tool renders)`
- `biome lint: 20 formatting/lint errors (mostly unused template literal, formatting diffs in 3 source files)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
