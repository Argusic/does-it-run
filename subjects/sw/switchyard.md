# Switchyard

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NVIDIA-NeMo/Switchyard, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/switchyard

## Pinned environment

- Project commit: `6f4e7749083a86484a0140078a42d487aed7259e`
- Test commit: `6f4e7749083a86484a0140078a42d487aed7259e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 9.7 to 15.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 9.7 | 1 | 1 | [run](https://argusic.com/run/758b827a-c803-442b-9291-2638574b3da7) |
| 2 | pass | 100 | 13 | 15.7 | 4 | 4 | [run](https://argusic.com/run/abfc69ed-0257-4a94-b81f-87527a7f0af1) |

## What was observed on a clean machine

Attempt 1:

- `Missing libpython3.12-dev system package prevents prefill-router tests from linking (rust-lld: unable to find library -lpython3.12) and prevents cargo test for switchyard-py and switchyard-node`

Attempt 2:

- 1 min: `uv not found in PATH after pip install`
- 2 min: `cargo not found in PATH for pytest`
- 3 min: `libpython3.12-dev not installed (no root), pyo3-dependent crates cannot link`
- 1 min: `initial TOML config missing capable_target/efficient_target for auto route`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
