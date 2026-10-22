# sonus

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/evancohen/sonus, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/sonus

## Pinned environment

- Project commit: `efb3cfbc449fba8c22ae4f67592723f6c41c9bf7`
- Test commit: `efb3cfbc449fba8c22ae4f67592723f6c41c9bf7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 10.8 to 17.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 10.8 | 0 | 0 | [run](https://argusic.com/run/7171e92a-0d3d-4906-8616-3b8144b7cd20) |
| 2 | pass with mocks | 92 | 17 | 17.2 | 5 | 5 | [run](https://argusic.com/run/430aacc7-57f7-4277-a67e-fe8ed4b1bbbe) |

## What was observed on a clean machine

Attempt 2:

- 7 min: `snowboy native build failed: link error 'cannot find -lcblas' (no BLAS dev libs on host, no root)`
- 9 min: `grpc@1.24.11 (dep of @google-cloud/speech) had no prebuilt binary for Node 18 (ABI node-v109) and its source build failed missing zlib.h and zlib implementation`
- 1 min: `npm test (eslint 3.19 bin wrapper) fails on Node 18 with shelljs circular-dependency 'Bad substitution'`
- `No audio recorder binary (rec/sox/arecord) on host, so Sonus.start() cannot capture from a mic`
- `Real Google Cloud Speech streaming requires real service credentials; no keys available in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
