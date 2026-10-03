# dblab

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/danvergara/dblab, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/dblab

## Pinned environment

- Project commit: `3f586e739236d440fa091a2ddcfc5300490260b8`
- Test commit: `3f586e739236d440fa091a2ddcfc5300490260b8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 8.7 to 27.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 3.5 | 27.2 | 3 | 3 | [run](https://argusic.com/run/09d8a631-4121-44e6-a518-5a9edb62a110) |
| 2 | pass with mocks | 92 | 8 | 8.7 | 0 | 0 | [run](https://argusic.com/run/78ebfe70-d360-45de-b002-e31b7a8aa476) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `V compiler not available in container`
- `Test suite fails to compile , 12 test files use legacy pre-rename V language syntax (inline type struct in function bodies, array literal syntax) incompatible with v0.5.2 compiler`
- `App binary outputs to TUI terminal only , --version and --help produce no stdout/stderr text because cobra/bubbletea writes directly to /dev/tty`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
