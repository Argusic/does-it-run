# jobseeker-analytics

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JustAJobApp/jobseeker-analytics, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/jobseeker-analytics

## Pinned environment

- Project commit: `4f494e396f1a042b667b2f19c3e3bb3db13978e4`
- Test commit: `4f494e396f1a042b667b2f19c3e3bb3db13978e4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 7 | 2 | 2 | [run](https://argusic.com/run/c6e0857c-ce0c-40c7-9255-1aa1b827c5ce) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `psycopg2==2.9.10 requires pg_config to build from source (no PostgreSQL dev headers available)`
- 4 min: `spacy-cleaner==3.2.1 requires spacy<3.5.0 but en-core-web-sm model requires spacy>=3.7.2`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
