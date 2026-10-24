# vectorlite

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/1yefuwang1/vectorlite, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/vectorlite

## Pinned environment

- Project commit: `cb976eea0848e5a91b0dc46b41f553c83dfd0cc7`
- Test commit: `cb976eea0848e5a91b0dc46b41f553c83dfd0cc7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.3 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8.2 | 8.3 | 3 | 3 | [run](https://argusic.com/run/a1b019b8-df18-426f-8beb-e9930e177a24) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `ninja not found`
- 1 min: `zip/unzip not found (vcpkg dependency)`
- `ops_test: 2 float16 precision failures (InnerProduct_F16, Normalize_F32ToF16)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
