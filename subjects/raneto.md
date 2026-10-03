# Raneto

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ryanlelek/Raneto, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/raneto

## Pinned environment

- Project commit: `a42f280b7e49b92ee435ab6950428c69b498c12d`
- Test commit: `a42f280b7e49b92ee435ab6950428c69b498c12d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.6 to 9.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 9.6 | 3 | 3 | [run](https://argusic.com/run/1078b505-f5ff-4790-9240-30e4b020f103) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18 (installed) does not meet the project's engine requirement of >=23.14.0 , import.meta.dirname is not available in Node 18 causing crash on startup`
- 0.5 min: `server.js crashed after startup , server.address() returned null in Express 5, causing a TypeError reading 'port' on null`
- 0.5 min: `server.js had an unused 'server' variable that lint flagged`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
