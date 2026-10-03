# coze-studio

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coze-dev/coze-studio, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/coze-studio

## Pinned environment

- Project commit: `fefb05ff27be1da939612fbf9faf5db62583b8ae`
- Test commit: `fefb05ff27be1da939612fbf9faf5db62583b8ae`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 28.9 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/65603987-675f-46e4-b847-579b8f72fb29) |
| 2 | pass with mocks | 92 | 28.3 | 28.9 | 5 | 5 | [run](https://argusic.com/run/dcd2d516-7a7e-4fc4-a6a1-1b9df0827d1d) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `go binary not found in container`
- 5 min: `bytedance/sonic v1.15.0/loader links runtime.lastmoduledatap on Go 1.24.0`
- 3 min: `Node 18.19.1 installed but project requires >=21`
- 2 min: `NVM shell sourcing fails in sh environment`
- `5 test packages fail: api/handler/coze, domain/knowledge/service, domain/memory/database/service, domain/workflow/internal/compose/test, infra/rdb/impl/rdb`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
