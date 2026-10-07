# react-router

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/remix-run/react-router, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/react-router

## Pinned environment

- Project commit: `246ddbeced9c2a02bd1de6ae87c5b6ce17225755`
- Test commit: `246ddbeced9c2a02bd1de6ae87c5b6ce17225755`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 84.7 to 84.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 44 | 84.7 | 2 | 2 | [run](https://argusic.com/run/0c9cbc8e-b613-4fe2-9f32-cc8ee3ff3745) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js 18.19.1 is below the required >=22.22.0`
- `Flaky timeout in special-characters-test.tsx when run in full suite (2 tests failed once)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
