# Uptimer

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/VrianCao/Uptimer, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/uptimer

## Pinned environment

- Project commit: `7bbe5191b31ae7b66fc088a7641861885f19bb0d`
- Test commit: `7bbe5191b31ae7b66fc088a7641861885f19bb0d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.8 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 6.8 | 0 | 0 | [run](https://argusic.com/run/d10c6e2d-bfcd-469d-b3d6-38b77c7999fb) |
| 2 | pass | 100 | 6 | 9.8 | 5 | 5 | [run](https://argusic.com/run/3592fe85-b167-4d28-984e-d2b13256d223) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Node.js v18.19.1 installed but project requires >=22.14.0`
- 0.5 min: `pnpm not found on system`
- 0.5 min: `wrangler not globally installed`
- 0.5 min: `Port 8787 was held by a left-over workerd process from a prior session`
- `Unauthenticated admin request (no Bearer token) returns 500 instead of 401`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
