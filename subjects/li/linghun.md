# Linghun

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/linghungegeg/Linghun, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/linghun

## Pinned environment

- Project commit: `05d8457bd04aa1b0eec4608e4effccf799bd43ad`
- Test commit: `05d8457bd04aa1b0eec4608e4effccf799bd43ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 74.3 to 74.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 86 | 1.5 | 74.3 | 10 | 7 | [run](https://argusic.com/run/f845f1e6-8010-401d-9d21-a9fb31c0b4de) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `model-doctor-runtime: test expected English 'not configured/not-sent' but code now outputs Chinese '未生效'`
- 3 min: `tui-interaction-contract: Todo test expected individual task summary that doesn't exist in refactored createTodoSurfacePreview`
- 2 min: `tui-interaction-contract: ProductBlock test checked for removed code pattern in refactored component`
- 3 min: `mcp-index-runtime: bundled codebase-memory binary is Git LFS pointer, not real binary`
- 2 min: `failure-learning-runtime: Windows path test fails on Linux because basename doesn't parse backslashes`
- 2 min: `index-runtime: Windows artifact path test fails on Linux because path.join uses forward slashes`
- 2 min: `view-model: TERM=dumb in test environment causes early return before LINGHUN_TERMINAL_TIER override`
- `index.test.ts: 113 complex integration test failures (pre-existing)`
- `tools/src/index.test.ts: 4 failures (pre-existing)`
- `tui-permission-runtime.test.ts: 2 failures (pre-existing)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
