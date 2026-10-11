# expo-github-action

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/expo/expo-github-action, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/expo-github-action

## Pinned environment

- Project commit: `eab7a230208c952974db8c3245cfd78402c7b385`
- Test commit: `eab7a230208c952974db8c3245cfd78402c7b385`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.6 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 4.6 | 2 | 2 | [run](https://argusic.com/run/43639b13-c402-411d-95e5-477dcbbb3f2e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `tests failed with TS2304: Cannot find name 'jest' / TS2593: Cannot find name 'describe' in all 12 test suites`
- 2 min: `build script ncc.js failed because bun is not installed and prebuild step deleted node_modules`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
