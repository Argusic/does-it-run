# opencrew

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AlexAnys/opencrew, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/opencrew

## Pinned environment

- Project commit: `7937758b701693f8f3577081e74c1ccdb268a660`
- Test commit: `7937758b701693f8f3577081e74c1ccdb268a660`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.4 to 13.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 13.4 | 4 | 4 | [run](https://argusic.com/run/8fb29fae-7c2d-4c18-8888-9598b1c3a4f3) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node 18.19.1 is too old - openclaw requires >=24.16.0`
- 1 min: `npm install -g failed EACCES`
- 1 min: `Config validation: agents.ownership required for multi-agent, session.agentToAgent unrecognized`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
