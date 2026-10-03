# pear-desktop

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pear-devs/pear-desktop, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pear-desktop

## Pinned environment

- Project commit: `8bd5c312a19f8f337fc65ff13955c4f587bd2df6`
- Test commit: `8bd5c312a19f8f337fc65ff13955c4f587bd2df6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 4.3 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 4.3 | 3 | 3 | [run](https://argusic.com/run/d9f75fb5-57a1-494a-89ca-57949d187425) |
| 2 | pass | 100 | 5 | 4.4 | 0 | 0 | [run](https://argusic.com/run/15b4593c-0298-4e3b-bdf0-6d2c2ad96f0a) |
| 3 | pass with mocks | 92 | 3 | 7.7 | 3 | 3 | [run](https://argusic.com/run/0cfcad1a-09be-4246-bf53-9a5c07acd408) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18 is incompatible with node-gyp@13.0.0 which requires ^22.22.2 || ^24.15.0 || >=26.0.0`
- 1 min: `pnpm 9.2.0 is too old; project requires pnpm >=11`
- 0.5 min: `pnpm start fails: SUID chrome-sandbox not correctly configured (requires root)`

Attempt 3:

- 1 min: `Node.js v18 was too old (requires >=22, pnpm >=11). System had Node 18.19.1 and no pnpm.`
- 1 min: `Electron SUID sandbox helper not configured (expected: non-root container).`
- `Playwright integration test expects music.youtube.com URL but app loads a Google login page first (no real auth session in container).`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
