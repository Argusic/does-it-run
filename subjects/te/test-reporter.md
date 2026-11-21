# test-reporter

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dorny/test-reporter, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/test-reporter

## Pinned environment

- Project commit: `2f9230a92bfadd838bacfa65e26e2f973f08f108`
- Test commit: `2f9230a92bfadd838bacfa65e26e2f973f08f108`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 1.3 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 1.3 | 0 | 0 | [run](https://argusic.com/run/223a4b61-5b53-418c-a82c-503283afe4fb) |
| 2 | pass with mocks | 92 | 2 | 5.9 | 2 | 2 | [run](https://argusic.com/run/646a2e93-325a-487f-a3d6-bca4061bfc10) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `System Node.js is v18.19.1 but the repo requires node >=24 (engines and .nvmrc v24); npm ci/typescript/jest failed to work correctly`
- 1 min: `First app launch failed with 'Unable to access summary file: /tmp/ghsum/summary.md' because GITHUB_STEP_SUMMARY file did not exist`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
