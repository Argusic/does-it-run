# primp

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deedy5/primp, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/primp

## Pinned environment

- Project commit: `84c1c45d614d2085192826409517e813ecf461f1`
- Test commit: `84c1c45d614d2085192826409517e813ecf461f1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.6 to 14.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 22 | 14.6 | 5 | 4 | [run](https://argusic.com/run/945c5559-b4d9-46c7-a56d-870c60a4cde1) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `No Rust toolchain in container`
- 6 min: `System Python lacks libpython3.12 dev library; pyo3 cdylib link failed (rust-lld unable to find -lpython3.12)`
- 1 min: `PEP 668 externally-managed environment blocked pip install`
- 4 min: `cargo test --workspace fails linking primp-python libtest against system python (env gap)`
- 1 min: `cargo clippy --all-targets -D warnings fails on pre-existing primp-h2 test lints`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
