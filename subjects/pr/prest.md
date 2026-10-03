# prest

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/prest/prest, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/prest

## Pinned environment

- Project commit: `9070bda7e9ab6b6484e04a0983b8afd61c8315e6`
- Test commit: `9070bda7e9ab6b6484e04a0983b8afd61c8315e6`
- Worker image digest: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 21.4 to 21.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 17 | 21.4 | 4 | 4 | [run](https://argusic.com/run/5eb041f8-608e-4c57-9cc1-94d7cc468b85) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not installed in container`
- 1 min: `gcc missing for -race flag in unit tests`
- 7 min: `docker not available for integration test stack`
- 2 min: `Missing ICU/SSL runtime libs for embedded postgres`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
