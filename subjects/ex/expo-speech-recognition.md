# expo-speech-recognition

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jamsch/expo-speech-recognition, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/expo-speech-recognition

## Pinned environment

- Project commit: `faee6cddcfdc025aedb7d494984922b3627b7c8a`
- Test commit: `faee6cddcfdc025aedb7d494984922b3627b7c8a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 53.4 to 53.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 53.4 | 2 | 2 | [run](https://argusic.com/run/24f91d47-d7d4-40c7-8d52-9cc2cc48e3fb) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `System Node v18.19.1 is below Expo/Metro's required >=20.19.4 (configs.toReversed is not a function)`
- 2 min: `Root npm test has no test files (expo-module jest exits 1 with 'No tests found')`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
