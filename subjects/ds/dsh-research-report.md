# dsh-research-report

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PerryLink/dsh-research-report, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dsh-research-report

## Pinned environment

- Project commit: `baa17487745ecfa24a8ee300dc3f6505c1df645b`
- Test commit: `baa17487745ecfa24a8ee300dc3f6505c1df645b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.7 to 1.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 1.7 | 1 | 1 | [run](https://argusic.com/run/97c51b72-c294-43ac-9be8-1cc55f9139da) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js v18.19.1 below project minimum Node ^22.19.0 || >=24.0.0; pnpm not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
