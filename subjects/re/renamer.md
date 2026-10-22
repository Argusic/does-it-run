# renamer

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/75lb/renamer, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/renamer

## Pinned environment

- Project commit: `72e984e567e739676944cd41acbd0182a185ab0c`
- Test commit: `72e984e567e739676944cd41acbd0182a185ab0c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.2 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 4.2 | 2 | 2 | [run](https://argusic.com/run/fa40ff54-785d-4674-b068-e2e73f5a5afb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Test runner @75lb/nature missing`
- 1 min: `Test expects ANSI codes but chalk disables them in non-TTY`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
