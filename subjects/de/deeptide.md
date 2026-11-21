# deeptide

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/paean-ai/deeptide, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/deeptide

## Pinned environment

- Project commit: `b48688d56c3eb61d0c028de2fa73dd674be2f3e8`
- Test commit: `b48688d56c3eb61d0c028de2fa73dd674be2f3e8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 5.5 to 10 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 10 | 3 | 3 | [run](https://argusic.com/run/c72d1cd2-1b8a-465e-92b3-77cd93731cf4) |
| 2 | fail | 80 | 5 | 5.5 | 2 | 2 | [run](https://argusic.com/run/cece692d-bdde-4eff-8ab1-604d835d2c9f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not installed`
- 2 min: `Bun not installed (no unzip binary)`
- 1 min: `Mock server script had syntax error in HTTPServer invocation`

Attempt 2:

- 0.2 min: `Rust toolchain not pre-installed in container`
- `Cargo.toml warnings: redundant homepage field in all 4 crate manifests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
