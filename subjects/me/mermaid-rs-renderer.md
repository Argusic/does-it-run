# mermaid-rs-renderer

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/1jehuang/mermaid-rs-renderer, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/mermaid-rs-renderer

## Pinned environment

- Project commit: `3726ccbffe0e8032361eb9668694b24f77858060`
- Test commit: `3726ccbffe0e8032361eb9668694b24f77858060`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 54.5 to 54.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 54.5 | 2 | 2 | [run](https://argusic.com/run/6466c264-13af-4e0c-a4a3-89c420d2265e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain not installed (rustc, cargo missing)`
- 1 min: `quadrant_point_label_bboxes_stay_inside_canvas assertion failed: point.y - point.label.height / 2.0 >= 0.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
