# agentbox

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/madarco/agentbox, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/agentbox

## Pinned environment

- Project commit: `605ee75d63319003c188bc532d4e5b2ba36a51d6`
- Test commit: `605ee75d63319003c188bc532d4e5b2ba36a51d6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19.1 to 19.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 19.1 | 3 | 3 | [run](https://argusic.com/run/6b8976fb-9508-4814-b4cc-c4e164cfac21) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 does not satisfy engines.node >=20.10`
- 1 min: `pnpm binary not found on PATH`
- 3 min: `rsync binary not found, causing 9 test failures in sandbox-core`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
