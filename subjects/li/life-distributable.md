# life-distributable

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mattabate/life-distributable, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/life-distributable

## Pinned environment

- Project commit: `2b222c753fba6e6375837cb1048173d4db56364f`
- Test commit: `2b222c753fba6e6375837cb1048173d4db56364f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.7 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 11.7 | 3 | 3 | [run](https://argusic.com/run/b8af42a6-90b3-404b-bc5e-2311f3af03de) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go 1.26 compiler not installed on system`
- 1 min: `Go std lib not in compiler tree (split package)`
- `codesign not found (macOS-only tool)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
