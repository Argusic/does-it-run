# dao-code

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tigicion/dao-code, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dao-code

## Pinned environment

- Project commit: `48da0890eb652bbbc09d0fe1e874ca86c58ea96e`
- Test commit: `48da0890eb652bbbc09d0fe1e874ca86c58ea96e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.9 to 10.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 10.9 | 2 | 2 | [run](https://argusic.com/run/872f95a2-0b5e-426a-b483-3d9d39140427) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18 system-installed, requires Node >=20 per package.json engines field`
- 0.5 min: `Flaky TUI test failures in App.test.tsx (timing-dependent assertion for '对话导航' and 'Theme switched' strings) , pass on re-run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
