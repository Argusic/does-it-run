# xleak

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bgreenwell/xleak, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/xleak

## Pinned environment

- Project commit: `ef6560c8e16815e2e74acf3973c0a5958a2c6523`
- Test commit: `ef6560c8e16815e2e74acf3973c0a5958a2c6523`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 4.3 | 0 | 0 | [run](https://argusic.com/run/f361c4cc-fb8b-499c-9954-179bfe817431) |
| 2 | pass | 100 | 1.5 | 4 | 2 | 2 | [run](https://argusic.com/run/76d43e4a-1762-4682-8f7c-077013b0548b) |

## What was observed on a clean machine

Attempt 2:

- 0.3 min: `Rust toolchain not installed`
- 0.2 min: `openpyxl missing (test fixture generator)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
