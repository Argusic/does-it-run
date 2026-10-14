# movary

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/leepeuker/movary, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/movary

## Pinned environment

- Project commit: `9953a06fae563b6e26292e0987f8cab7e6a2b942`
- Test commit: `9953a06fae563b6e26292e0987f8cab7e6a2b942`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 36.7 to 36.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 36.7 | 3 | 3 | [run](https://argusic.com/run/6711761a-b859-4fe1-b7ac-552f3f3558a7) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No PHP or Composer available in container`
- 4 min: `Composer 2.10+ fails because FrankenPHP sets argv[0] to its own binary path`
- 3 min: `Psalm cannot run due to same argv[0] issue with Symfony Console CLI parser`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
