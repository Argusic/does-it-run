# fast-plaid

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lightonai/fast-plaid, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/fast-plaid

## Pinned environment

- Project commit: `df2be46ee930d066507a813208e4cfd1117eac74`
- Test commit: `df2be46ee930d066507a813208e4cfd1117eac74`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 31 to 31 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7.4 | 31 | 5 | 5 | [run](https://argusic.com/run/5d09bf10-197f-4104-a76b-cc95e974c8f8) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `Rust toolchain (rustc, cargo) not installed in container`
- 1 min: `Python development headers (Python.h) missing , no python3-dev package installed`
- 0.3 min: `tch-rs 0.20.0 compilation failed with torch 2.14.1+ C++ API differences (e.g. symint::sizes, deprecated functions)`
- 0.2 min: `patchelf binary not available for maturin wheel bundling`
- 1.5 min: `Segfault on importing the .so , maturin bundles renamed copies of torch shared libraries (different SONAMEs) that conflict with already-loaded torch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
