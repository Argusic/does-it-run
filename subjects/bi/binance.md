# binance

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sieblyio/binance, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/binance

## Pinned environment

- Project commit: `12bd77bf5e28b443a346671d7df8d12a5dae41b9`
- Test commit: `12bd77bf5e28b443a346671d7df8d12a5dae41b9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 3.2 to 4.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 4.7 | 1 | 1 | [run](https://argusic.com/run/2a7e65d7-4dfd-4cd3-9606-3d9b1dd3f5a1) |
| 2 | pass with mocks | 92 | 0.17 | 3.2 | 3 | 3 | [run](https://argusic.com/run/2a15e46b-eabe-4b31-a908-2c1f3fb75056) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `9 test suites fail: require real Binance API credentials (HMAC/RSA/ED25519 keys) not available in this container`

Attempt 2:

- `Node.js v18.19.1 below .nvmrc requirement v24.18.0 - npm install emitted EBADENGINE warnings for eslint, rimraf, and brace-expansion`
- `Binance API returns HTTP 451 from this container location - network.test.ts 4 tests fail with 'Service unavailable from a restricted location'`
- `Auth and private endpoint tests require env vars API_KEY_COM/API_SECRET_COM which are not set`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
