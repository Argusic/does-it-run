# elastic-ci-stack-for-aws

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/buildkite/elastic-ci-stack-for-aws, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/elastic-ci-stack-for-aws

## Pinned environment

- Project commit: `da710c6403bca1fd2bd4d95712afae194e9e49a8`
- Test commit: `da710c6403bca1fd2bd4d95712afae194e9e49a8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.3 to 24.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 24.3 | 2 | 2 | [run](https://argusic.com/run/2d373673-e2f8-4cb0-b8f4-80d4a983bfa8) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Test fixer.go had hardcoded Docker paths (/code/...) and used 'nobody' user requiring root`
- 8 min: `Go compiler not present in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
