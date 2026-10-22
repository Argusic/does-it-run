# app-examples

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/miroapp/app-examples, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/app-examples

## Pinned environment

- Project commit: `e51fb9b06e02f4cf02fe258fef49ef3be1d85038`
- Test commit: `e51fb9b06e02f4cf02fe258fef49ef3be1d85038`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.9 to 7.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 7.9 | 3 | 3 | [run](https://argusic.com/run/fd16dd60-3699-4ecb-aeae-c49baf52aeeb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `yarn command not found in container`
- 1 min: `Python pip fails with externally-managed-environment`
- 1 min: `node-passport-oauth hardcodes empty clientID/clientSecret`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
