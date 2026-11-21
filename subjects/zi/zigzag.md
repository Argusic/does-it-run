# zigzag

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/simpsoka/zigzag, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/zigzag

## Pinned environment

- Project commit: `429a028054145fc3e541525bb05b57596fa49d22`
- Test commit: `429a028054145fc3e541525bb05b57596fa49d22`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.6 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 13 | 14.2 | 2 | 0 | [run](https://argusic.com/run/eaf2b6d2-db2f-41d8-9696-461af17974fc) |
| 2 | pass | 100 | 3.5 | 5.6 | 0 | 0 | [run](https://argusic.com/run/1f6d96e3-ceea-4c2f-9308-0dc68ba60b15) |

## What was observed on a clean machine

Attempt 1:

- `lettering::editing_tests::text_is_sewn_the_same_wherever_its_moved: assertion failed - run 0: 184 stitches for 183 after moving text by (128.6, -44.1). Pre-existing bug in repo single commit.`
- `lettering::tests::text_is_selected_with_shift_arrows_double_clicks_drags_and_typed_over: unwrap() on None at lettering.rs:1739. Pre-existing bug in repo single commit.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
