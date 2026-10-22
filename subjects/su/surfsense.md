# SurfSense

**Verdict: runs.** Argusic Score 66.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MODSetter/SurfSense, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/surfsense

## Pinned environment

- Project commit: `176aed261a24a85d217538960e91c59746561bd2`
- Test commit: `176aed261a24a85d217538960e91c59746561bd2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 20 to 21.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 46 | 22 | 21.2 | 5 | 4 | [run](https://argusic.com/run/4930d3d7-cd53-486b-844c-69c917b969b8) |
| 2 | pass | 86.67 | 8 | 20 | 3 | 1 | [run](https://argusic.com/run/8adefa42-1b07-4621-a802-a1aceabea8ac) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Node.js v18 installed but surfsense_web requires 24.x; pnpm install failed for @rocicorp/zero-sqlite3 due to missing readline/readline.h`
- 1 min: `uv not installed`
- 1 min: `pnpm not installed (npm install -g rejected by OS permissions)`
- 2 min: `Backend Config class fails at module level: AutoEmbeddings.get_embeddings(None)`
- `SDK test expects 'Connection refused' but kernel returns 'Cannot assign requested address'`

Attempt 2:

- 1 min: `surfsense_backend tests fail without EMBEDDING_MODEL env var (AutoEmbeddings.get_embeddings(None) fails)`
- 3 min: `surfsense_web (Next.js) needs Node 24.x but only 18.19.1 is available; @rocicorp/zero-sqlite3 native module fails to compile`
- 2 min: `plugins/remote/host test_scaling.py, test_progress.py, test_results.py, test_plugin_lifespans.py hang (need browser/scraping infra)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
