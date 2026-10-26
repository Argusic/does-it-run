# DeepSeek-Bot

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Fei2411/DeepSeek-Bot, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/deepseek-bot

## Pinned environment

- Project commit: `1bebe826f74e9a72cabafd3b80602b05af867b38`
- Test commit: `1bebe826f74e9a72cabafd3b80602b05af867b38`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.3 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3.4 | 5.3 | 4 | 4 | [run](https://argusic.com/run/8d7b0b5c-7641-4f8c-8a2a-35204605a1ba) |

## What was observed on a clean machine

Attempt 1:

- 0.4 min: `Node.js v18 is too old; project requires Node 22+ for 'registerHooks' from 'node:module'`
- 0.5 min: `oxlint native binding @oxlint/binding-linux-x64-gnu not installed by 'npm run harness' on Node 18`
- `Desktop app (Electron) prints DBus errors in container without system bus`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
