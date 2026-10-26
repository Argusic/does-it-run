# esp-v2

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GoogleCloudPlatform/esp-v2, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/esp-v2

## Pinned environment

- Project commit: `e81efd39d2c2cd1074b97fee24f50f9005bbd81a`
- Test commit: `e81efd39d2c2cd1074b97fee24f50f9005bbd81a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.1 to 11.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 11.1 | 1 | 1 | [run](https://argusic.com/run/9b4c3e51-6d7f-48b0-8d63-b7c72673be99) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing clang-14 C++ compiler required for Bazel/Envoy C++ build. The .bazelrc hardcodes CC=clang-14.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
