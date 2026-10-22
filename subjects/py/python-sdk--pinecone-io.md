# python-sdk

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pinecone-io/python-sdk, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/run/fba43e2a-5928-4049-98d2-22f5d380b701

## Pinned environment

- Project commit: `f9550510fa076ff7c9bbccd310ceaa7c57c0ffd6`
- Test commit: `f9550510fa076ff7c9bbccd310ceaa7c57c0ffd6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 36.1 to 56.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 56.8 | 0 | 0 | [run](https://argusic.com/run/fba43e2a-5928-4049-98d2-22f5d380b701) |
| 2 | pass with mocks | 92 | 20 | 36.1 | 1 | 1 | [run](https://argusic.com/run/2507dc73-2dd3-466c-a790-43332815037a) |

## What was observed on a clean machine

Attempt 2:

- 6 min: `cargo build failed: protoc binary not found (prost-build requires it to compile rust/proto/db_data_2026-07.proto)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
