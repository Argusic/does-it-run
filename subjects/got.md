# got

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sindresorhus/got, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/got

## Pinned environment

- Project commit: `e1d87d2ced01d5b7d855a7dc8b091bf7b014a1e4`
- Test commit: `e1d87d2ced01d5b7d855a7dc8b091bf7b014a1e4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 44.9 to 60.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 60.7 | 0 | 0 | [run](https://argusic.com/run/b81ddc23-d633-4778-8274-2d9c79a4ef76) |
| 2 | pass | 100 | 25 | 44.9 | 5 | 5 | [run](https://argusic.com/run/adf403e3-e62a-413f-9941-be0d463652d8) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `System Node.js v18 does not satisfy engine requirement >=22`
- 5 min: `Initial Node.js v22.0.0 too old for dnsOrder 'ipv6first' and ALPN callback APIs`
- 5 min: `Test server binds to 0.0.0.0; direct connection fails with EADDRNOTAVAIL in Docker container`
- 5 min: `1 pre-existing test failure in test/timings.ts - 'cached DNS lookups reuse resolved addresses in timing requests'`
- 1 min: `npm install warnings about unsupported engines (node versions) for several devDependencies`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
