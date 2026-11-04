# E2B

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/e2b-dev/E2B, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/e2b

## Pinned environment

- Project commit: `ccaf9fc0ffe6ac39c7ec786af7608ab1de19467b`
- Test commit: `ccaf9fc0ffe6ac39c7ec786af7608ab1de19467b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 10.1 to 33 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 33 | 33 | 3 | 3 | [run](https://argusic.com/run/8bc7c243-c865-48db-9424-94cd2f6d5128) |
| 2 | pass with mocks | 92 | 9 | 10.1 | 4 | 4 | [run](https://argusic.com/run/65dfdaf5-a8d0-4925-97fb-58f57fa0d15a) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pnpm not on PATH (node v18.19.1 bundled)`
- 1 min: `uv not installed`
- `No E2B_API_KEY in environment`

Attempt 2:

- 2 min: `pnpm and uv were not installed; container Node 18.19.1 did not meet repository Node >=22 requirement`
- 3 min: `CLI template create with COPY failed: Cannot find package 'glob' imported from packages/cli/dist/index.js`
- 2 min: `CLI template create with COPY then failed: Cannot find package 'tar' imported from packages/cli/dist/index.js`
- 2 min: `Credential-dependent template-create test failed before test execution when E2B_API_KEY was absent`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
