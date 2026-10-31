# dsh-wallpaper-engine

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elysia395/dsh-wallpaper-engine, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dsh-wallpaper-engine

## Pinned environment

- Project commit: `7ba44b2424e55b70fe28fea753a7abf27ae7cdb3`
- Test commit: `7ba44b2424e55b70fe28fea753a7abf27ae7cdb3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 72.3 to 72.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 72.3 | 5 | 5 | [run](https://argusic.com/run/21cb6e1a-abf6-40a5-87aa-c50a7c8aa17b) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node was v18.19.1 (plugin requires >=22.12) and the shipped dsh 0.1.7-rc.2 CLI silently no-ops on Node 22.14 because its bin.js gate is import.meta.main (undefined before Node 24); dsh --version printed empty`
- 2 min: `node scripts/install-source.mjs failed at 'dsh plugin add' with ERR_PNPM_ADDING_TO_ROOT because the profile pnpm workspace declares packages: ['.']; neither the --ignore-workspace-root-check flag nor the workspace yaml key took effect throu`
- 4 min: `No system Chromium; the container lacks user namespaces so Chromium needs --no-sandbox`
- 1 min: `Full verify chain hung under Node 24 at test/verify-upload-store.mjs after printing ALL UPLOAD-STORE CHECKS PASSED (35)`
- 1 min: `dsh web exited right after printing the token URL when it tried to open the default browser`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
