# saltcorn

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/saltcorn/saltcorn, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/saltcorn

## Pinned environment

- Project commit: `c296aa3d463fc07038ac508820bad72016bedbb7`
- Test commit: `c296aa3d463fc07038ac508820bad72016bedbb7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.5 to 44.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 29 | 44.5 | 4 | 4 | [run](https://argusic.com/run/49bcbfb5-77e3-4603-8970-4ccb36427624) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm install fails with ERESOLVE due to @fonticonpicker/react-fonticonpicker requiring react 16 vs workspace react 18`
- 2 min: `Node.js version 18.19.1 installed but project requires >=20`
- 3 min: `Static import of @saltcorn/sqlite-mobile/sqlite_capacitor in db/index.ts triggers ERR_REQUIRE_ESM on Node 18 (CJS module requiring ESM)`
- 2 min: `Server cluster workers crash on SQLite backend`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
