# quiver

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/varkor/quiver, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/quiver

## Pinned environment

- Project commit: `2f289ecbae9b7e5a473e04b924750c538ed5c4cf`
- Test commit: `2f289ecbae9b7e5a473e04b924750c538ed5c4cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.2 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 6.2 | 2 | 2 | [run](https://argusic.com/run/e38e6a5b-5e3a-496e-92ea-ff8f847a1ffa) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `unzip not found; couldn't extract KaTeX zip`
- 0.2 min: `service-worker.js missing (HTTP 404)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
