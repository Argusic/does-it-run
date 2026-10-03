# agent-scan

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/snyk/agent-scan, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agent-scan

## Pinned environment

- Project commit: `2527530b842e681404a8daad06c65f1973fc90c8`
- Test commit: `2527530b842e681404a8daad06c65f1973fc90c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 34.2 to 34.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 34.2 | 1 | 1 | [run](https://argusic.com/run/49f30766-040f-4153-9f53-70d186bc9a48) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `20 tests failing (8 unit, 12 e2e): SnykTokenError: SNYK_TOKEN environment variable not set`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
