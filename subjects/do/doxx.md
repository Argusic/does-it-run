# doxx

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bgreenwell/doxx, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/doxx

## Pinned environment

- Project commit: `062819a10f423f2b2ce52be6d264e9069b1b9a40`
- Test commit: `062819a10f423f2b2ce52be6d264e9069b1b9a40`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.2 to 11.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 9.2 | 1 | 1 | [run](https://argusic.com/run/6ed57a12-4666-47a1-9c83-2227ec3e2aaf) |
| 2 | pass | 100 | 7 | 11.8 | 1 | 1 | [run](https://argusic.com/run/240f60bb-be7c-4fc2-bb77-7ba7e89e1611) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `NO_COLOR=1 env var causes crossterm 0.28 to suppress all ANSI color output in tests, causing 2 test failures`

Attempt 2:

- 15 min: `ANSI color export tests failed because crossterm 0.28's Display impl for SetForegroundColor produces only \x1b[m instead of \x1b[38;5;Nm or \x1b[38;2;R;G;Bm, causing test_ansi_export_color_depths and test_ansi_export_formatting to fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
