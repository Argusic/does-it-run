# openclaw-setup

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tuanminhhole/openclaw-setup, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/openclaw-setup

## Pinned environment

- Project commit: `b8f073533cd8bd1280fb3f317f955e82a2ab2d0f`
- Test commit: `b8f073533cd8bd1280fb3f317f955e82a2ab2d0f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.6 to 5.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 2 | 5.6 | 2 | 1 | [run](https://argusic.com/run/0008b2b8-fbcf-4d1d-8d24-d4e8610d891e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js 18.19.1 lacks built-in node:sqlite module required by local-server.js`
- 1 min: `npm test fails: docs_dev/ directory is gitignored and not shipped, test scripts not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
