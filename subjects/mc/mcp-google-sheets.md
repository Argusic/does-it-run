# mcp-google-sheets

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xing5/mcp-google-sheets, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mcp-google-sheets

## Pinned environment

- Project commit: `b2f98244590f1d0982505f4faa908731278ea998`
- Test commit: `b2f98244590f1d0982505f4faa908731278ea998`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 4.6 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 4.6 | 0 | 0 | [run](https://argusic.com/run/a0803da8-ea02-4d63-a209-1f45d94d9bab) |
| 2 | pass with mocks | 92 | 5 | 5.4 | 1 | 1 | [run](https://argusic.com/run/4c964070-7a4c-419a-872a-719f798e4dee) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Real Google Cloud credentials required for live API calls (service_account JSON with valid private key + Google Cloud project)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
