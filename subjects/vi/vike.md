# vike

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vikejs/vike, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vike

## Pinned environment

- Project commit: `b163fd9a896ea9affd30aec162b3609b2f8184d5`
- Test commit: `b163fd9a896ea9affd30aec162b3609b2f8184d5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12 to 44.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 12 | 3 | 3 | [run](https://argusic.com/run/81047691-cafc-44bf-b184-c245636604f9) |
| 2 | pass | 100 | 41 | 44.9 | 1 | 1 | [run](https://argusic.com/run/a386c2da-dac2-454a-be0a-3189e34eab06) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 was installed but Vike requires >=20.19.0`
- 1 min: `pnpm not installed globally; npm install failed due to EACCES (writes to /usr/local)`
- 1 min: `Initial pnpm install with Node v18 skipped optional native binding @rolldown/binding-linux-x64-gnu, causing vitest startup error`

Attempt 2:

- 6 min: `docs preview e2e crashed with 'JavaScript heap out of memory' (exit 134) during docs build under Node's default 2GB V8 heap`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
