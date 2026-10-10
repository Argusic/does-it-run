# knowledge

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RobRoyce/knowledge, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/knowledge

## Pinned environment

- Project commit: `dcab981af9e0caa15d80b383cdcbf69e38a39f4d`
- Test commit: `dcab981af9e0caa15d80b383cdcbf69e38a39f4d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.5 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 8.5 | 1 | 1 | [run](https://argusic.com/run/99784fd6-219a-4c26-93d2-3ae565ab137a) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Node.js 18.19.1 found, project requires 24+ for node:sqlite`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
