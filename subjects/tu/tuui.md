# tuui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AI-QL/tuui, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tuui

## Pinned environment

- Project commit: `0be513448dc674c76581e84bb1ff0a3a0be104c7`
- Test commit: `0be513448dc674c76581e84bb1ff0a3a0be104c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.7 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.34 | 3.7 | 1 | 1 | [run](https://argusic.com/run/ecc47fbc-a79b-4541-9c67-7ae530f7e022) |

## What was observed on a clean machine

Attempt 1:

- 0.18 min: `Node.js v18.19.1 installed but project requires >=22.12.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
