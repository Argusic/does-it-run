# professional-programming

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/charlax/professional-programming, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/professional-programming

## Pinned environment

- Project commit: `c482301495112980792614b4089aa0624ba6e51e`
- Test commit: `c482301495112980792614b4089aa0624ba6e51e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 3.6 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 5 | 10.2 | 2 | 2 | [run](https://argusic.com/run/f40373f4-91ae-48bd-b4b4-73d9ae59e881) |
| 2 | fail | 20 | 0 | 3.6 | 1 | 1 | [run](https://argusic.com/run/fadf65ad-2054-4264-a9fa-1b7589117cec) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pre-commit hook 'black' (rev 19.3b0) failed with ImportError: cannot import name '_unicodefun' from 'click'`
- 2 min: `pre-commit hook 'doctoc' (v1.4.0) failed with ENOENT on file with spaces in name`

Attempt 2:

- `Repository is a curated reading list (charlax/professional-programming) with no package manager, build system, test suite, or application to install/launch - purely markdown documentation with 3 illustrative Python scripts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
