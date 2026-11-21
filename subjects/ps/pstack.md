# pstack

**Verdict: runs with mocks.** Argusic Score 88.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/backnotprop/pstack, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pstack

## Pinned environment

- Project commit: `059190ea76d062acc19b9d733e9096d7be35081c`
- Test commit: `059190ea76d062acc19b9d733e9096d7be35081c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 5.9 to 13.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.4 | 5.9 | 4 | 4 | [run](https://argusic.com/run/84574fa7-9e60-4b16-86c3-394a9c2becfc) |
| 2 | pass with mocks | 85.33 | 0.5 | 13.7 | 3 | 2 | [run](https://argusic.com/run/de2b805b-ce24-4682-8652-075f69996e83) |

## What was observed on a clean machine

Attempt 1:

- `statechart tests: 5 tests fail because node:module.registerHooks() (Node 22+) is not available on Node 18.19.1`
- `statechart tests: 1 test fails because String.prototype.toWellFormed() (Node 19+) is not available on Node 18.19.1`
- `poteto-mode tests require bun, which is not installed`
- `skills CLI (npx skills) requires Node 22.20+`

Attempt 2:

- 2 min: `Package.json test script uses --disable-warning flag unsupported in Node 18`
- 3 min: `Test helper uses String.prototype.toWellFormed() requiring Node 20+`
- `CLI and pipeline tests need Node 22+ or Java/TLC for full environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
