# aichat

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sigoden/aichat, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/aichat

## Pinned environment

- Project commit: `82976d349ad97ac9aae0655ad631dace5e2a6385`
- Test commit: `82976d349ad97ac9aae0655ad631dace5e2a6385`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.3 to 7.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 7.3 | 1 | 1 | [run](https://argusic.com/run/e7c59418-0ed7-437e-bba5-05e798d4fc51) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not pre-installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
