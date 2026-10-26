# respan-gateway

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/respanai/respan-gateway, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/respan-gateway

## Pinned environment

- Project commit: `c9e433b35c6fa94b9abebf3064e298d96fbf8f38`
- Test commit: `c9e433b35c6fa94b9abebf3064e298d96fbf8f38`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 9.8 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9.5 | 9.8 | 2 | 2 | [run](https://argusic.com/run/3f7229b3-fe94-499b-b232-8834215db94e) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `Ubuntu 24.04 system Python blocks pip install (PEP 668 externally-managed-environment)`
- `Rust workspace default build includes Python extension crate which needs libpython3.12-dev for linking`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
