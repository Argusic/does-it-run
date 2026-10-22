# onchain-dex-cli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/outsmartchad/onchain-dex-cli, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/onchain-dex-cli

## Pinned environment

- Project commit: `1851d27b71a25fcef793d321ab3e077cce0bf0e8`
- Test commit: `1851d27b71a25fcef793d321ab3e077cce0bf0e8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.9 to 8.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 8.9 | 2 | 2 | [run](https://argusic.com/run/dded64ab-e45e-448a-87f7-215ab2ecf856) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 below project requirement (>=20)`
- 4 min: `8 test suites need PRIVATE_KEY + MAINNET_ENDPOINT env vars for real Solana RPC calls with structured on-chain pool state data`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
