# IncarnaMind

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/junruxiong/IncarnaMind, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/incarnamind

## Pinned environment

- Project commit: `aebaa3d0e6930c2e67b9bba2d85b6d9fb576a1c1`
- Test commit: `aebaa3d0e6930c2e67b9bba2d85b6d9fb576a1c1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.7 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 6.7 | 3 | 3 | [run](https://argusic.com/run/25d7c853-78a3-4aed-9308-7834575cd90a) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Container has Node.js 18 but project requires >=24`
- 0.5 min: `Electron sandbox helper not configured correctly in container (SUID sandbox)`
- 0.5 min: `Built-in resources (skills, examples, notices) not in output directory`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
