# d2-vscode

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/d2lang/d2-vscode, licensed BSD-3-Clause, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/d2-vscode

## Pinned environment

- Project commit: `23346fb575b1eb309b75a331315d4424e99a2fb1`
- Test commit: `23346fb575b1eb309b75a331315d4424e99a2fb1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.6 to 7.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 7.6 | 3 | 3 | [run](https://argusic.com/run/bc9b71d8-4253-4ff4-965c-ccf859947b46) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `yq (YAML-to-JSON converter) not available for regenerating syntax grammar from YAML source`
- 1.5 min: `@vscode/vsce 4.x requires Node.js >=20, system Node is 18`
- 0.5 min: `vsce deps (undici) require File global not available in Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
