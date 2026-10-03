# trieve

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/devflowinc/trieve, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/trieve

## Pinned environment

- Project commit: `a99b21e23f21025757b44efb594676c4a7b7495f`
- Test commit: `a99b21e23f21025757b44efb594676c4a7b7495f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.3 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 12.5 | 12.3 | 6 | 3 | [run](https://argusic.com/run/14b8f842-b7db-4fbe-86a9-e3426f40baea) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Python SDK missing 'requests' dependency (missing from pyproject.toml deps but needed at runtime)`
- 0.5 min: `Python SDK import artifact: 'from traitlets import default' in dataset_configuration_dto.py (unused, not in SDK's dep tree)`
- 0.5 min: `yarn install fails on Node 18 due to 'conf@14.0.0' requiring Node >=20`
- `No Rust toolchain (cargo/rustc) , Rust server cannot build`
- `No Docker daemon , Docker services (Postgres, Qdrant, Redis, etc.) cannot start`
- `Network to api.trieve.ai is unreachable , TS SDK integration tests and live server verification impossible`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
