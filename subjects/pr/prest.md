# prest

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/prest/prest, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/prest

## Pinned environment

- Project commit: `9070bda7e9ab6b6484e04a0983b8afd61c8315e6`
- Test commit: `9070bda7e9ab6b6484e04a0983b8afd61c8315e6`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 3.8 to 21.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 17 | 21.4 | 4 | 4 | [run](https://argusic.com/run/5eb041f8-608e-4c57-9cc1-94d7cc468b85) |
| 2 | pass | 100 | 2 | 3.8 | 0 | 0 | [run](https://argusic.com/run/3f0501bb-11ae-4c1d-8dfd-c4000c718e3c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not installed in container`
- 1 min: `gcc missing for -race flag in unit tests`
- 7 min: `docker not available for integration test stack`
- 2 min: `Missing ICU/SSL runtime libs for embedded postgres`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
