# tach

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tach-org/tach, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/tach

## Pinned environment

- Project commit: `65df67ac51a8d0e8f9e0398ea72c924fea34fd25`
- Test commit: `65df67ac51a8d0e8f9e0398ea72c924fea34fd25`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8 to 8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12.5 | 8 | 3 | 3 | [run](https://argusic.com/run/6d5fdb4f-52f9-4222-b0f6-543ee3ea49a1) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No Rust toolchain (rustc/cargo/maturin not in PATH)`
- 0.5 min: `Detached HEAD in git repo causes test_export_report_diagnostics to fail`
- 7 min: `Version mismatch: pyproject.toml has 0.35.1 but pip-installed CLI reports 0.35.2`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
