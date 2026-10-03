# dejavu

**Verdict: runs with mocks.** Argusic Score 79.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/appbaseio/dejavu, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dejavu

## Pinned environment

- Project commit: `8b8f11f40cd60bef953442c4ad9ac913f3d3cd5c`
- Test commit: `8b8f11f40cd60bef953442c4ad9ac913f3d3cd5c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 3; wall time 11.7 to 24.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 11 | 11.7 | 3 | 3 | [run](https://argusic.com/run/319fa645-bd8c-402a-a1f3-f232ca6acd7c) |
| 2 | pass with mocks | 72 | 3 | 24.7 | 1 | 0 | [run](https://argusic.com/run/d252ee80-b5ae-4634-a7b4-f569891eab9f) |
| 3 | pass with mocks | 85.33 | 24 | 24.3 | 3 | 2 | [run](https://argusic.com/run/19056d75-639f-47c8-a2b9-ce4be3cf40d8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `yarn package manager not found in container`
- 1 min: `missing 'favicons' peer dependency for favicons-webpack-plugin`
- 1 min: `git submodule 'batteries' repositories not initialized (empty directories)`

Attempt 2:

- `Import warning: persistElasticsearchServerlessFlavor not found in constants/config (build warning only, non-blocking)`

Attempt 3:

- 2 min: `favicons peer dependency requires Node >= 20.9.0, container has 18.19.1`
- 3 min: `source tests in batteries submodule can't be transformed by Jest , no submodule babel config`
- `2 mappings tests fail: batteries submodule updated updateMapping() (commit 50a23dc) but test expectations are stale`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
