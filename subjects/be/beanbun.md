# Beanbun

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kiddyuchina/Beanbun, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/beanbun

## Pinned environment

- Project commit: `092063908d5831a6cb660748b1f2f49b62afcdc6`
- Test commit: `092063908d5831a6cb660748b1f2f49b62afcdc6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.3 to 16.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 16.3 | 2 | 2 | [run](https://argusic.com/run/947cc50e-529c-43ab-9932-dc8bf3e33665) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP missing from container`
- 8 min: `Composer not available (PHP built without phar extension, complex dep chain)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
