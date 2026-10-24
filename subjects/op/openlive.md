# openlive

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/katipally/openlive, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openlive

## Pinned environment

- Project commit: `849173cd1c8c17a95d600b17b428c301722bf5df`
- Test commit: `849173cd1c8c17a95d600b17b428c301722bf5df`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.7 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 3.7 | 3 | 3 | [run](https://argusic.com/run/4dd0d210-9737-44f9-bf1a-282986d56b47) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node v18.19.1 installed but project requires >=22.13`
- 0.5 min: `pnpm not found on PATH`
- 0.2 min: `free-ports.mjs requires lsof or ss (not in minimal container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
