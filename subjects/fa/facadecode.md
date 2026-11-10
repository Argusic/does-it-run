# facadecode

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/y5ez3g/facadecode, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/facadecode

## Pinned environment

- Project commit: `d630a3dc904e68e3dacf774fe7cd4b3d0008c3eb`
- Test commit: `d630a3dc904e68e3dacf774fe7cd4b3d0008c3eb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 31.8 to 31.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 31.8 | 3 | 3 | [run](https://argusic.com/run/26c8474c-88b7-4ba4-bac7-4fbd2189abe3) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `npm test hangs on glob expansion; individual file runs succeed`
- 3 min: `npm run test for extension: 2 timeout failures in execution.test.js (1) and ptyd.test.js (1) - cleanup hooks timing out after successful test assertions`
- 3 min: `IDE npm install fails: kerberos native module requires gssapi/gssapi.h (libkrb5-dev system package), not installable without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
