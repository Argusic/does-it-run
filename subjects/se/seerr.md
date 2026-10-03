# seerr

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/seerr-team/seerr, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/seerr

## Pinned environment

- Project commit: `6f5a17735d383b110cca04326ecd536ad7675ed6`
- Test commit: `6f5a17735d383b110cca04326ecd536ad7675ed6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 8.7 to 16.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 16.1 | 0 | 0 | [run](https://argusic.com/run/2a323ec2-ef00-479b-a4e0-21845b28bb01) |
| 2 | pass | 100 | 2.5 | 8.7 | 0 | 0 | [run](https://argusic.com/run/ca9fbb10-a018-43bf-978d-76ed8b8fa6cf) |
| 3 | pass with mocks | 92 | 13 | 14.2 | 1 | 1 | [run](https://argusic.com/run/654873c5-0a4e-46be-870d-233cc8e831c1) |

## What was observed on a clean machine

Attempt 3:

- 6 min: `Node.js v18.19.1 installed but project requires ^22.19.0; pnpm v9.2.0 installed but requires ^10.0.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
