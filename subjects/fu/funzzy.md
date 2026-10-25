# funzzy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cristianoliveira/funzzy, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/funzzy

## Pinned environment

- Project commit: `a229380a3d4d4401ada0b75e88284eb98e48266a`
- Test commit: `a229380a3d4d4401ada0b75e88284eb98e48266a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.6 to 8.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 8.6 | 1 | 1 | [run](https://argusic.com/run/8baab45a-cd9e-443b-8080-428b894d0782) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `Two flaky tests failed due to coarse filesystem mtime granularity (the test wrote a file then checked for mtime change within the same clock tick)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
