# lapce

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lapce/lapce, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/lapce

## Pinned environment

- Project commit: `b604d57de4a820006d335a3be0d7583eb8fab558`
- Test commit: `b604d57de4a820006d335a3be0d7583eb8fab558`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 20.8 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/9910d7ac-9a7d-42e5-9f5a-aa56c8e9f762) |
| 2 | pass | 100 | 17 | 20.8 | 3 | 3 | [run](https://argusic.com/run/b38bdb49-5333-4801-a02b-21875fdb5e46) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `Rust toolchain not installed (rustc: not found)`
- 0.5 min: `Cannot install system dev packages via apt (no root, lock denied)`
- `Vulkan: no GPU drivers found in container (vkCreateInstance: Found no drivers)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
