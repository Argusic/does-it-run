# mcp-n8n-workflow-builder

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/salacoste/mcp-n8n-workflow-builder, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/mcp-n8n-workflow-builder

## Pinned environment

- Project commit: `ba48196ba4d06e67dafe1b1200628a40d764f73b`
- Test commit: `ba48196ba4d06e67dafe1b1200628a40d764f73b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.3 to 2.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 2.3 | 1 | 1 | [run](https://argusic.com/run/414ce1a6-4ae3-44eb-9913-a7113d729e76) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `TypeScript build error: Property 'includes' does not exist on type 'string | number | true | string[] | AxiosHeaders' in src/utils/responseValidation.ts:46`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
