# Kiri

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GaoSSR/Kiri, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/run/09e02ae3-bf45-471c-a47d-ec6f06e5883c

## Pinned environment

- Project commit: `e7495fc80d9db393e55ac9f6f148da584a32fc8b`
- Test commit: `e7495fc80d9db393e55ac9f6f148da584a32fc8b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.2 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.2 | 5.2 | 1 | 1 | [run](https://argusic.com/run/09e02ae3-bf45-471c-a47d-ec6f06e5883c) |

## What was observed on a clean machine

Attempt 1:

- `ss/lsof not installed in container - port detection limited`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
