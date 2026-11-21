# OrcaReplay

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Continuum-AI-Corp/OrcaReplay, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/orcareplay

## Pinned environment

- Project commit: `a9178ca26af95cfd3231b8eb2da4ae11dbbd0a84`
- Test commit: `a9178ca26af95cfd3231b8eb2da4ae11dbbd0a84`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 16.3 to 22.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 16.3 | 2 | 2 | [run](https://argusic.com/run/e8b019f5-c0cb-49cc-bfc9-f7b321812253) |
| 2 | pass | 100 | 2 | 22.5 | 1 | 1 | [run](https://argusic.com/run/42d74e87-29a6-4313-a582-1c53122a13ff) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18.19.1 below minimum required version (^20.19.0 || >=22.12.0)`
- 1 min: `'python' command not found, only 'python3' available; tests hardcode 'python' as interpreter`

Attempt 2:

- 1 min: `'python' binary not found (only 'python3'), causing spawn ENOENT in 5 tests that launch Python agents`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
