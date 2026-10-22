# ngx-scanner

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zxing-js/ngx-scanner, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ngx-scanner

## Pinned environment

- Project commit: `db43c139ec15f5b6973dbacb643b99342bd70eed`
- Test commit: `db43c139ec15f5b6973dbacb643b99342bd70eed`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.1 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 10.1 | 6 | 6 | [run](https://argusic.com/run/f0f876a3-b692-4045-958a-4020aaf03454) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 too old for Angular CLI 22 (requires v22.22.3+)`
- 1 min: `Angular CLI detected yarn not in PATH, refused to run`
- 3 min: `No Chrome browser installed in container`
- 1 min: `Chrome crashpad_handler binary not executable (rw-rw-r--)`
- 1 min: `Chrome sandbox unusable (no user namespaces in container)`
- 1 min: `npm install failed with peer dependency conflict on @angular/animations`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
