# bla

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/qybaihe/bla, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/bla

## Pinned environment

- Project commit: `eb44984a5c3e1920bec9c7bdc8403c6d93d0bc0e`
- Test commit: `eb44984a5c3e1920bec9c7bdc8403c6d93d0bc0e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 2.8 | 1 | 1 | [run](https://argusic.com/run/2dc66bee-b927-4876-9700-5a566215f0eb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Test 'also discovers root-level artifacts when dist/ already exists' in harden-autodiscover.test.ts fails: BLA SQLite support requires Node.js 22.x >=22.13.0 or Node.js >=24.0.0 with node:sqlite enabled (current runtime: v18.19.1)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
