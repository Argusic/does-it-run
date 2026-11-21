# SearchCLI

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/volcengine/SearchCLI, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/searchcli

## Pinned environment

- Project commit: `2d757a9cb783aca87039b2cb6dd5125336fd71fa`
- Test commit: `2d757a9cb783aca87039b2cb6dd5125336fd71fa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 1.8 to 2.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 1.8 | 0 | 0 | [run](https://argusic.com/run/3b676686-29e9-4ec3-ba0b-f712670d641b) |
| 2 | pass with mocks | 92 | 2 | 2.1 | 1 | 1 | [run](https://argusic.com/run/f7da46d9-2046-4700-9179-aeb15efb172b) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `Node.js v18.19.1 in container does not meet the >=20 requirement`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
