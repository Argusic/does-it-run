# tapo

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mihai-dinculescu/tapo, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/tapo

## Pinned environment

- Project commit: `282bd233f50f71593d511aca911d7a92719ad41a`
- Test commit: `282bd233f50f71593d511aca911d7a92719ad41a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 9.9 to 11.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 11.3 | 0 | 0 | [run](https://argusic.com/run/f76d7bd9-1f0f-4b20-90db-71d75f59aa1b) |
| 2 | pass with mocks | 92 | 15 | 9.9 | 3 | 3 | [run](https://argusic.com/run/26c13be6-9406-499a-b667-dcd5972ce880) |

## What was observed on a clean machine

Attempt 2:

- `Rust toolchain not installed in container (rustc: not found)`
- 2 min: `maturin develop --release failed: no virtualenv found outside venv`
- `maturin develop --release inside venv failed: pip install --group flag not supported by this pip version`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
