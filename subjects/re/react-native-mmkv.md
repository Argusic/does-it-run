# react-native-mmkv

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/margelo/react-native-mmkv, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/react-native-mmkv

## Pinned environment

- Project commit: `ca5acf0ca9acc5cd1b75c486be6adad40c488047`
- Test commit: `ca5acf0ca9acc5cd1b75c486be6adad40c488047`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 2.7 to 4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 4 | 1 | 1 | [run](https://argusic.com/run/d3b7f2e9-7e3e-4dc4-ac90-97dbf2f259ca) |
| 2 | pass | 100 | 0.12 | 2.7 | 0 | 0 | [run](https://argusic.com/run/cd6c1932-4053-450c-a0b8-bfac795d0828) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `bun is not available. The postinstall script ("bun mmkv build") fails. The repo uses bun as its package manager, but only npm is installed and installing bun globally requires root.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
