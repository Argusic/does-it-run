# Endoplexity

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Endokelp/Endoplexity, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/endoplexity

## Pinned environment

- Project commit: `315e0d89e035a76c90efdec110c3673b86625308`
- Test commit: `315e0d89e035a76c90efdec110c3673b86625308`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.6 to 2.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 2.6 | 1 | 1 | [run](https://argusic.com/run/e2169be2-5cbf-40b9-9231-0cbbe6febc8f) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Node.js v18.19.1 in container, but project requires Node >=24 (type stripping experimental feature)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
