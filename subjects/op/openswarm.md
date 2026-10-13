# OpenSwarm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Intrect-io/OpenSwarm, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openswarm

## Pinned environment

- Project commit: `47da9ed0c10c399240732e3d99642e5b642bf099`
- Test commit: `47da9ed0c10c399240732e3d99642e5b642bf099`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 47.8 to 47.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 48 | 47.8 | 7 | 7 | [run](https://argusic.com/run/60595e08-ce2a-489e-8712-fbc7a95442d8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 incompatible with engine requirement >=22`
- 1 min: `Missing @rolldown/binding-linux-x64-gnu native addon`
- 2 min: `better-sqlite3 compiled for Node 18 (ABI 108), not Node 22 (ABI 127)`
- 2 min: `Sharp optional dependency missing linux-x64 binary`
- 2 min: `tsc not found on PATH when diagnosticsTool tests create temp directories`
- 15 min: `bubblewrap (bwrap) not installed, sandbox verification fails closed`
- 1 min: `git-lfs not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
