# embedJs

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/llm-tools/embedJs, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/embedjs

## Pinned environment

- Project commit: `fe778606d66a933934937bb44b4c729cc9b4606c`
- Test commit: `fe778606d66a933934937bb44b4c729cc9b4606c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11 to 11 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 11 | 2 | 2 | [run](https://argusic.com/run/1d9cb6a8-d626-4ee1-a19b-c8714be39c51) |

## What was observed on a clean machine

Attempt 1:

- `npm EBADENGINE warnings: ~25 transitive deps require Node>=20 but container has 18.19.1`
- 2 min: `node_modules/@llm-tools symlinks point to .ts source dirs, not dist .js output, causing ERR_MODULE_NOT_FOUND at runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
