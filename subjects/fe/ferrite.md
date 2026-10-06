# Ferrite

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OlaProeis/Ferrite, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/ferrite

## Pinned environment

- Project commit: `3ba085c561670342d72c560efbf6b0b92b5c0b46`
- Test commit: `3ba085c561670342d72c560efbf6b0b92b5c0b46`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 48.7 to 48.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12.5 | 48.7 | 3 | 3 | [run](https://argusic.com/run/c7032a4e-9df7-4458-9026-2ad466144099) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain not installed`
- 1.5 min: `fontconfig.pc not found (libfontconfig-dev missing, cannot install without root)`
- 8 min: `42 test compilation errors: missing imports and missing method to_markdown`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
