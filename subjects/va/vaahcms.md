# vaahcms

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/webreinvent/vaahcms, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/vaahcms

## Pinned environment

- Project commit: `8d7898f7a385a5fade1180a9b664ff158d873129`
- Test commit: `8d7898f7a385a5fade1180a9b664ff158d873129`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.8 to 20.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 20.8 | 5 | 5 | [run](https://argusic.com/run/7b24a89f-5e2c-46c7-ac27-5f616844c7dd) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `PHP and Composer not installed in container`
- 2 min: `Missing composer dependency ZanySoft/LaravelZip`
- 1 min: `Missing composer dependency intervention/image`
- 3 min: `User/UserBase models hardcode mysql connection, causing boot crash with SQLite`
- 2 min: `npx vaah cms:install CLI failed (Observable polyfill missing + interactive prompts)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
