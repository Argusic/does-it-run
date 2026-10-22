# Frame

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kaanozhan/Frame, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/frame

## Pinned environment

- Project commit: `fb4731434b0be3d3115d273983d7f8b6a0851659`
- Test commit: `fb4731434b0be3d3115d273983d7f8b6a0851659`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.4 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.25 | 12.4 | 2 | 2 | [run](https://argusic.com/run/8a71f5e0-e52a-4d2c-967b-600f2fb3d5f4) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `test/envPath.test.js: loginShell never answers /bin/sh , the test assumed passwd entry would never be /bin/sh, but in this container os.userInfo().shell returns /bin/sh`
- 5 min: `test/structureRead.test.js: 'unknown' freshness test used readDescriptor , on this filesystem with coarse mtime precision, the stat-based check doesn't always detect the rewrite`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
