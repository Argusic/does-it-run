# onenote

**Verdict: runs.** Argusic Score 91 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/patrikx3/onenote, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/onenote

## Pinned environment

- Project commit: `a9666c8221e01a37700d29b359e1d74136595a62`
- Test commit: `a9666c8221e01a37700d29b359e1d74136595a62`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 3.8 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 0.4 | 3.8 | 2 | 1 | [run](https://argusic.com/run/d9eea3b7-f2c5-41d5-8450-7f280f516020) |
| 2 | pass with mocks | 92 | 7 | 7 | 3 | 3 | [run](https://argusic.com/run/a8fdd1c4-556c-4663-9bb9-8d2a30bbd079) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `vitest 4.1.8 requires Node >=20, which is not available (v18.19.1 is installed)`
- `electron binary could not install because @electron/get v5.0.0 requires Node >=22.12.0`

Attempt 2:

- 2 min: `Node.js v18.19.1 is too old; project requires Node >= v22.12.0. vitest/rolldown also requires newer Node`
- 1 min: `vitest/rolldown missing platform native binding @rolldown/binding-linux-x64-gnu`
- 2 min: `Electron binary not downloaded because install.js uses require() for ESM module @electron/get, which fails on older Node`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
