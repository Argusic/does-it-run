# danghuangshang

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wanikua/danghuangshang, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/danghuangshang

## Pinned environment

- Project commit: `acea185a9a1abb1788206fddc9c52a2693afaa39`
- Test commit: `acea185a9a1abb1788206fddc9c52a2693afaa39`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 19.1 to 19.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 19 | 19.1 | 3 | 3 | [run](https://argusic.com/run/90b214ee-1b29-4dc5-b4ab-23f6454f5831) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 too old (package.json requires >=22.19.0, openclaw requires >=24.16.0)`
- 1 min: `context-compressor.js module missing exports (estimateTokens, compressConversation, generateSummary) needed by manual test suite`
- 1 min: `OpenClaw Gateway crash-loop breaker tripped from repeated interrupted starts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
