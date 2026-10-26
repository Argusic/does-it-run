# EPlusTV

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tonywagner/EPlusTV, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/eplustv

## Pinned environment

- Project commit: `10dd938b8ec1ec43cc92e15f459eee293f62aaf1`
- Test commit: `10dd938b8ec1ec43cc92e15f459eee293f62aaf1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.2 to 9.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8.3 | 9.2 | 3 | 3 | [run](https://argusic.com/run/95077434-16fe-4b35-9240-2f8c9e3f1f53) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `npm ci exit 2: 'Bad substitution' from husky prepare script in sh`
- `yt-dlp binary missing (not on PATH)`
- `TypeScript 4.4.3 cannot parse cheerio@1.0.0 / jsdom@26.0.0 types (TS1005 on ???)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
