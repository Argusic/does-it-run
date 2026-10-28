# bitbucket-cli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/avivsinai/bitbucket-cli, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/bitbucket-cli

## Pinned environment

- Project commit: `5068ddc2961cb05279c1a6fbcdd583328867c728`
- Test commit: `5068ddc2961cb05279c1a6fbcdd583328867c728`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 20 | 2.9 | 1 | 1 | [run](https://argusic.com/run/1e95c63a-cdd1-4af6-9483-6d19688ece8d) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No Go toolchain installed in container (go: not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
