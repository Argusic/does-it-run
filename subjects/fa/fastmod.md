# fastmod

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/facebookincubator/fastmod, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/fastmod

## Pinned environment

- Project commit: `974e3ef60b784d3eea9b2a214ac0079957415230`
- Test commit: `974e3ef60b784d3eea9b2a214ac0079957415230`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.4 to 7.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 7.4 | 1 | 1 | [run](https://argusic.com/run/6c25b545-3f2b-46ee-af39-28e9df21b331) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Cargo.toml: clap dependency missing 'derive' feature needed for derive macros (Parser, command, arg)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
