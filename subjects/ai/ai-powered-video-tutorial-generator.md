# AI-Powered-Video-Tutorial-Generator

**Verdict: runs.** Argusic Score 98 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AkshitIreddy/AI-Powered-Video-Tutorial-Generator, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-powered-video-tutorial-generator

## Pinned environment

- Project commit: `9c260890214df68ad8fd0d681d3e77a6a7b7ea9f`
- Test commit: `9c260890214df68ad8fd0d681d3e77a6a7b7ea9f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 22 to 34 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 7 | 34 | 5 | 4 | [run](https://argusic.com/run/1b4f94f8-65ec-4551-84ee-dcab0eb2796d) |
| 2 | pass | 100 | 15 | 22 | 4 | 4 | [run](https://argusic.com/run/8a9c6c5f-4abc-4504-a1a7-3c5bc77ecbde) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Python 3.12.3 does not match pinned 3.12.13`
- 1 min: `uv 0.12.17 not matching pinned 0.12.7`
- 2 min: `install-manifest.json has stale file sizes for local_presenter_worker.py (14916 vs actual 15519)`
- `Desktop TS test: asks for explicit cast fails , cannot find 'Select Daniel · software instructor' button in JSDOM`
- `Tauri native build fails: too many open files, no WebView2`

Attempt 2:

- 3 min: `Node.js v18.19.1 found, need v24.20.0`
- 2 min: `pnpm not found`
- 1 min: `uv not found`
- 1 min: `esbuild build script blocked by pnpm`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
