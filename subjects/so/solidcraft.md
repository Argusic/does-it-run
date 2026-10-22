# solidcraft

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tangency-labs/solidcraft, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/solidcraft

## Pinned environment

- Project commit: `6422ef84d513343ae46434a6053fc530b44e17fb`
- Test commit: `6422ef84d513343ae46434a6053fc530b44e17fb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 62.8 to 62.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 61 | 62.8 | 2 | 1 | [run](https://argusic.com/run/ff06b09a-047b-4ba5-a801-d6fc1200370f) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `OOM (SIGKILL) during cadmpeg_ir compilation with default profile (756MB RAM insufficient for opt-level 2)`
- `Kernel/sketch/engine/doc test suites run extremely slowly on this hardware (>5 min each) under memory pressure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
