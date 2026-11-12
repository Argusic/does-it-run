# grasp

**Verdict: runs.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cocofhu/grasp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/grasp

## Pinned environment

- Project commit: `796b6f297992f3cb59784df3572d8edaaef30ad1`
- Test commit: `796b6f297992f3cb59784df3572d8edaaef30ad1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.2 to 18.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 92 | 17 | 18.2 | 5 | 3 | [run](https://argusic.com/run/4050ffe1-1e88-410f-9647-a4d71ecec99f) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `go not found in container; server module requires Go 1.25+`
- 2 min: `node v18.19.1 present but web CI requires Node 24`
- `docker and docker compose not found; default README ./start.sh stack cannot run without root`
- 1 min: `first server launch used wrong env name GRASP_SERVER_PORT and listened on 8080`
- `server logs warn on boot: sql converting argument $1 type: unsupported type models.ProjectNotifyPolicy (notify policy channelIds backfill failed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
