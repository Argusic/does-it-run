# xs

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cablehead/xs, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/xs

## Pinned environment

- Project commit: `3473cb4fcb8e99f02a19fef0ea77890548d42c28`
- Test commit: `3473cb4fcb8e99f02a19fef0ea77890548d42c28`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 10.4 to 12.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 2.5 | 10.4 | 1 | 0 | [run](https://argusic.com/run/f1842e29-4feb-40fd-8671-91a9b421f965) |
| 2 | pass | 100 | 12 | 12.9 | 1 | 1 | [run](https://argusic.com/run/48e9d059-65db-4eb6-bbdb-a7f39d3d8e16) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `test_bytestream_ping panics: system ping(1) not present in container`

Attempt 2:

- 2 min: `ping command not found, causing test_bytestream_ping failure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
