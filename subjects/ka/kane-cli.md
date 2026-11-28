# kane-cli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LambdaTest/kane-cli, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/kane-cli

## Pinned environment

- Project commit: `31075fdeec842335d7de2072147636304da33519`
- Test commit: `31075fdeec842335d7de2072147636304da33519`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.3 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 5.3 | 3 | 3 | [run](https://argusic.com/run/eb9d50cd-3a7a-4081-b3e8-87e32e9c6928) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `EACCES: permission denied to /usr/local/lib/node_modules/@testmuai`
- 1 min: `Node 18 below minimum requirement Node 20`
- 2 min: `Chrome/Chromium not found on system`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
