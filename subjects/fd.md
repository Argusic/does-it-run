# fd

**Verdict: runs.** Argusic Score 73.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sharkdp/fd, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/fd

## Pinned environment

- Project commit: `1765d0817b4e706141115b81c29a5965630e243a`
- Test commit: `1765d0817b4e706141115b81c29a5965630e243a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 2.9 to 8.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.7 | 2.9 | 0 | 0 | [run](https://argusic.com/run/16fae721-1771-4056-a210-17a65ee3e4fc) |
| 2 | fail | 20 | n/a | 8.2 | 0 | 0 | [run](https://argusic.com/run/45f5dc91-d027-4774-bdd4-f7c2171e8ca7) |
| 3 | pass | 100 | 8 | 6.3 | 1 | 1 | [run](https://argusic.com/run/9eb2bd16-8d55-445a-a2c9-5163d211bf53) |

## What was observed on a clean machine

Attempt 3:

- 1 min: `tikv-jemalloc-sys OOM-killed during build due to 2GB RAM limit`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
