# compozy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/compozy/compozy, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/compozy

## Pinned environment

- Project commit: `d2c33a6f37cf7b60c5a63b5da8b353a848e10186`
- Test commit: `d2c33a6f37cf7b60c5a63b5da8b353a848e10186`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 35.1 to 94.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 33 | 35.1 | 6 | 6 | [run](https://argusic.com/run/d9a2ac63-7d67-443d-b185-c5e8e3167a86) |
| 2 | timeout | none | n/a | 94.4 | 0 | 0 | [run](https://argusic.com/run/ff81cb75-cfad-4056-9ac7-b7c42d741c57) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go not installed in environment`
- 1 min: `Bun not installed; npm global install rejected due to permissions`
- 1 min: `Bun install script required unzip (not installed, no root)`
- 5 min: `vitest fork workers crashed with 'Cannot read properties of undefined (reading bind)' in undici decompress.js`
- 2 min: `npm install failed with ERESOLVE (typescript 6 vs openapi-typescript peer conflict)`
- 1 min: `npm install also failed with 'Unsupported URL Type workspace:*'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
