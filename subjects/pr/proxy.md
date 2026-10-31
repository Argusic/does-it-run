# proxy

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RelayPlane/proxy, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/proxy

## Pinned environment

- Project commit: `bdceda091cbc3e021febd68cf42cf548cecc227d`
- Test commit: `bdceda091cbc3e021febd68cf42cf548cecc227d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 18.6 to 18.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 20 | 18.6 | 5 | 5 | [run](https://argusic.com/run/8aef700c-ff06-4a81-abd8-3c77b5710d6b) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `nanoid v5 is ESM-only but @relayplane/core and other packages use require('nanoid') (CJS)`
- 2 min: `vitest.config.ts alias points to ../learning-engine/src/index.ts which doesn't exist`
- 3 min: `Missing 'default' export in @relayplane/* package.json exports`
- 2 min: `crypto global not available in Node 18 (crypto.randomUUID used in background-detector.test.ts)`
- 1 min: `tsx binary not in .bin directory (launcher.test.ts)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
