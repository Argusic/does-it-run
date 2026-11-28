# phulp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/reisraff/phulp, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/phulp

## Pinned environment

- Project commit: `59c400e04e28981aaac3dcfde251bcffc918ec8a`
- Test commit: `59c400e04e28981aaac3dcfde251bcffc918ec8a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.6 to 2.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.6 | 2 | 2 | [run](https://argusic.com/run/934b0db6-a0c5-4b53-bd56-b8fa655c91eb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP not installed in container`
- 1 min: `PHPUnit 5.7 incompatible with PHP 8.3`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
