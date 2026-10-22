# next-plaid

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lightonai/next-plaid, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/next-plaid

## Pinned environment

- Project commit: `00e26aae0006b322727db277672211d9a0e3ccec`
- Test commit: `00e26aae0006b322727db277672211d9a0e3ccec`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 14 | 1 | 1 | [run](https://argusic.com/run/e7e20e4d-9364-4b13-868c-9ec4510308ae) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
