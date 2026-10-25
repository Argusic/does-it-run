# agentfs-claude

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/run-llama/agentfs-claude, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/agentfs-claude

## Pinned environment

- Project commit: `135bf7393402d753b747f43667926cb1b27085be`
- Test commit: `135bf7393402d753b747f43667926cb1b27085be`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.2 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 6.2 | 6 | 6 | [run](https://argusic.com/run/b27cdd44-f3de-48f1-9e5e-45510c0f515b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 is too old for vitest 4.x (needs node:util.styleText, added in v21.7)`
- 1 min: `rolldown native binding missing: @rolldown/binding-linux-x64-gnu was not installed`
- 1 min: `LlamaParseReader constructed at module import time, throwing before tests could skip`
- 1 min: `esbuild postinstall skipped, causing runtime issues`
- 1 min: `Compiled test files in dist/ caused AgentFS database lock conflicts with src/ tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
