# scrapecraft

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ScrapeGraphAI/scrapecraft, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/scrapecraft

## Pinned environment

- Project commit: `24c85545d7db1c2805d65700f8dde758938d40cf`
- Test commit: `24c85545d7db1c2805d65700f8dde758938d40cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.9 to 13.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.2 | 13.9 | 1 | 1 | [run](https://argusic.com/run/59c42c80-54eb-44dd-8036-c92f03e4808b) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `bcrypt 5.0.0 incompatible with passlib 1.7.4 bcrypt hash initialization`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
