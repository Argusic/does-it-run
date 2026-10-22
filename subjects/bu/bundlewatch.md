# bundlewatch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bundlewatch/bundlewatch, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/bundlewatch

## Pinned environment

- Project commit: `95997ac3bdf7ff1e3ec75bf123a2b06051e39b7d`
- Test commit: `95997ac3bdf7ff1e3ec75bf123a2b06051e39b7d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.1 to 2.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.25 | 2.1 | 2 | 2 | [run](https://argusic.com/run/d910f7dd-e0c0-47ce-9dd7-1086d56538d6) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Snapshot mismatch: gzip size differed by environment (248.46KB vs 248.5KB)`
- 0.1 min: `yarn not available, Makefile targets expect it`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
