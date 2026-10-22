# thing-editor

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Megabyteceer/thing-editor, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/thing-editor

## Pinned environment

- Project commit: `695d0bd8246f4999e16d4ca9e5399f2de5f044de`
- Test commit: `695d0bd8246f4999e16d4ca9e5399f2de5f044de`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.2 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 7 | 6.2 | 5 | 5 | [run](https://argusic.com/run/6863522c-964c-4f13-b676-42063a364814) |
| 2 | pass | 100 | 30 | 9.7 | 3 | 3 | [run](https://argusic.com/run/20dade8f-0e1a-4888-bbc6-0b322a1cce9c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Electron SUID sandbox binary not configured correctly in container`
- 1 min: `EMFILE too many open files on file watcher`
- 1 min: `GPU initialization errors in headless container`
- `D-Bus errors (no system bus in container)`
- `TypeScript type-checking errors from generated runtime typings (GameClasses, ThingSceneAllMap, CurrentSceneType)`

Attempt 2:

- 2 min: `Electron SUID chrome-sandbox not configured (requires root) - app aborted with SIGTRAP`
- 1 min: `Electron renderer got ERR_CONNECTION_REFUSED on http://localhost:5173/ because the vite dev server died with the invoking shell`
- `npm run build (tsc && vite build) fails on editor auto-generated typings (prefabs-typing.ts, ThingSceneAllMap, GameClasses) that only exist at runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
