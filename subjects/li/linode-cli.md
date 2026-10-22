# linode-cli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/linode/linode-cli, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/linode-cli

## Pinned environment

- Project commit: `251dbbc6a3258884cad74bfdaac1a6062337e8d2`
- Test commit: `251dbbc6a3258884cad74bfdaac1a6062337e8d2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.1 to 2.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.25 | 2.1 | 1 | 1 | [run](https://argusic.com/run/61fb6fe8-c011-4250-80de-2ba811515a6d) |

## What was observed on a clean machine

Attempt 1:

- 0.15 min: `Baked spec file data-3 missing from repository and initial pip install , CLI could not load any commands`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
