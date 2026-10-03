# cocoindex

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cocoindex-io/cocoindex, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/cocoindex

## Pinned environment

- Project commit: `f1c1ba4a83d3da0e4201b11866383d20a913b813`
- Test commit: `f1c1ba4a83d3da0e4201b11866383d20a913b813`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13 to 13 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 13 | 5 | 5 | [run](https://argusic.com/run/5966bb89-76c5-44b0-a3b1-d8c19ec9b758) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv not installed in container`
- 1 min: `Rust toolchain not installed`
- 1 min: `cargo test fails linking libpython3.12 (system Python 3.12 lacks shared lib, venv uses Python 3.11)`
- 1 min: `maturin develop fails with 'No such file or directory'`
- `CLI test fails: cocoindex command not in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
