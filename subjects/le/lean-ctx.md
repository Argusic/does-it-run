# lean-ctx

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yvgude/lean-ctx, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/lean-ctx

## Pinned environment

- Project commit: `1f8d2d35812da540b68054435e3692725f131193`
- Test commit: `1f8d2d35812da540b68054435e3692725f131193`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 55.1 to 97.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 62 | 64.8 | 2 | 2 | [run](https://argusic.com/run/c90d3f9f-7dfd-4a62-9412-f8816a3e4334) |
| 2 | timeout | none | n/a | 97.1 | 0 | 0 | [run](https://argusic.com/run/ad1266a5-fe59-44b3-aa2b-46382d9a9d5a) |
| 3 | fail | 20 | n/a | 55.1 | 0 | 0 | [run](https://argusic.com/run/460c52d5-4682-41e2-93ca-aff9dc680289) |

## What was observed on a clean machine

Attempt 1:

- `cargo test --lib (lib test) hits 8GB cgroup memory limit during compilation of the test binary due to all tree-sitter grammar crates being linked. The test binary with --cfg test requires ~7.5GB+, exceeding the 8GB limit.`
- 2 min: `Rust toolchain not pre-installed in the container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
