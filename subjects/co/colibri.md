# colibri

**Verdict: runs.** Argusic Score 73.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JustVugg/colibri, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/colibri

## Pinned environment

- Project commit: `fd93c41aa6ae2c7d1cc1a1e2d6b79dbe6d341708`
- Test commit: `fd93c41aa6ae2c7d1cc1a1e2d6b79dbe6d341708`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 24.1 to 37.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 24.1 | 0 | 0 | [run](https://argusic.com/run/0b6685eb-dee9-4edb-a843-bb35ae7cce18) |
| 2 | fail | 60 | 29 | 29.9 | 4 | 0 | [run](https://argusic.com/run/9a10aba7-dfda-4958-a205-fe910e4a573a) |
| 3 | fail | 60 | 30 | 37.6 | 1 | 0 | [run](https://argusic.com/run/19f16fbb-1b69-4172-96da-a52d4d6e44f7) |

## What was observed on a clean machine

Attempt 2:

- `C test test_qwen36_tier_multidev fails: multi-GPU fake CUDA backend cannot simulate two devices reaching resident state during warmstart (3/4 CUDA-tier tests pass fine)`
- `Web dashboard build fails: Node.js 18 lacks node:util.styleText (requires Node 21+)`
- `Desktop app cannot build: Rust/Cargo toolchain not available`
- `No real model weights available for end-to-end inference verification (requires ~370 GB download)`

Attempt 3:

- `test_resource_plan.py: test_auto_tune_mtp_off_when_disk_low_hit writes 12 GB temp file and gets OOM-killed by the container's 8 GB cgroup memory limit`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
