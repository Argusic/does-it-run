# rust-rpxy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/junkurihara/rust-rpxy, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/rust-rpxy

## Pinned environment

- Project commit: `cc7a654a845ba4cb63989136c7108f1e2695e4a3`
- Test commit: `cc7a654a845ba4cb63989136c7108f1e2695e4a3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.1 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 10.1 | 3 | 3 | [run](https://argusic.com/run/0accbe28-b4ed-4009-b410-92743d002882) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No Rust toolchain in container (rustc/cargo absent)`
- 9 min: `rpxy exits ~2s after startup under this PTY harness when spawned with job-control shells`
- 2 min: `Background Python backend died when its shell exited`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
