# harness-remote

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/giuliastro/harness-remote, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/harness-remote

## Pinned environment

- Project commit: `ee9d315c7a3329ab6ef5588d1565210167d47a9d`
- Test commit: `ee9d315c7a3329ab6ef5588d1565210167d47a9d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.7 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 3.7 | 2 | 2 | [run](https://argusic.com/run/ed1f603d-cfab-483a-95ee-3014bb6f6aa5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 is installed but package.json requires >=20. npm emits EBADENGINE warnings on install and the web client's Vite build fails with 'ReferenceError: CustomEvent is not defined'`
- `Server endpoint /v1/sessions returns 400 'Internal error: spawn xdg-open ENOENT' because xdg-open is not available in headless container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
