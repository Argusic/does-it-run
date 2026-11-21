# agent-plugin

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ChatCut-Inc/agent-plugin, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/agent-plugin

## Pinned environment

- Project commit: `e9092062de42bffbf12927cefc6b572864434dd8`
- Test commit: `e9092062de42bffbf12927cefc6b572864434dd8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.2 to 1.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.05 | 1.2 | 0 | 0 | [run](https://argusic.com/run/a2077b81-866c-480c-a73a-0a6c55c80246) |
| 2 | pass | 100 | 0 | 1.8 | 1 | 1 | [run](https://argusic.com/run/0e64354d-0098-40b0-88b7-948f63e80db4) |

## What was observed on a clean machine

Attempt 2:

- `zip command not available in container; build.mjs --no-zip works, but ZIP creation fails`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
