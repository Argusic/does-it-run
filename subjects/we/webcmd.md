# webcmd

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agentrhq/webcmd, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/webcmd

## Pinned environment

- Project commit: `719a75786a43158d1a9112830797610cda68bb03`
- Test commit: `719a75786a43158d1a9112830797610cda68bb03`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.9 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 4.9 | 2 | 2 | [run](https://argusic.com/run/f3f352f4-c03b-4a92-afc9-9c15f8db5764) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 too old (project requires >=20.6.0)`
- 1 min: `webcmd binary not on PATH after first global install with old Node`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
