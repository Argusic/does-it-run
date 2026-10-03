# textual

**Verdict: runs.** Argusic Score 73.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Textualize/textual, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/textual

## Pinned environment

- Project commit: `06dbeef4bb70fb718236aa418ed658ef4667a126`
- Test commit: `06dbeef4bb70fb718236aa418ed658ef4667a126`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 8.7 to 38.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 32 | 38.9 | 4 | 4 | [run](https://argusic.com/run/78fed6ae-8321-4e10-8d55-27970389ae8f) |
| 2 | fail | 20 | n/a | 8.7 | 0 | 0 | [run](https://argusic.com/run/6b2c2d35-3529-4478-b248-f467401228a4) |
| 3 | pass | 100 | 2 | 14.3 | 2 | 2 | [run](https://argusic.com/run/19b13dba-68f0-4938-b3d2-e4a30f3b1f39) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PEP 668 externally-managed-environment blocks system pip`
- 5 min: `NO_COLOR=1 env causes render() utility to strip ANSI, breaking 3+ renderable tests and adding 'nocolor' pseudo-class`
- 1 min: `Missing textual-dev package causes 3 test failures (devtools client import fails)`
- 1 min: `Missing pytest-textual-snapshot plugin causes 2 test errors`

Attempt 3:

- 3 min: `NO_COLOR=1 env var set in container suppresses Rich ANSI escape codes, causing ~408 test failures`
- 2 min: `tree-sitter syntax extras not installed, 3 syntax-marked tests fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
