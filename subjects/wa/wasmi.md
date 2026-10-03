# wasmi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wasmi-labs/wasmi, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/wasmi

## Pinned environment

- Project commit: `2970aa871cc1001b57b267ccecdcd1e42306199e`
- Test commit: `2970aa871cc1001b57b267ccecdcd1e42306199e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.3 to 22.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 42 | 22.3 | 2 | 2 | [run](https://argusic.com/run/6f52bacd-9ea9-4f8a-aa95-40dcc75bcba2) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Rust toolchain not pre-installed in container`
- 2 min: `git submodules not initialized; wast crate failed with 358 errors referencing missing .wast files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
