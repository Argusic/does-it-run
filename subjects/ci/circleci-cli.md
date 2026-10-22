# circleci-cli

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CircleCI-Public/circleci-cli, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/circleci-cli

## Pinned environment

- Project commit: `a2e7dd1c5b90822bbc408655ae23b840d8d46ca1`
- Test commit: `a2e7dd1c5b90822bbc408655ae23b840d8d46ca1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27.3 to 27.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 27.3 | 2 | 2 | [run](https://argusic.com/run/f67d1ee5-15e3-4adf-8b0c-6ac1f404dae5) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go compiler not installed in container`
- 6 min: `go test -race compilation timeout (>5 min)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
