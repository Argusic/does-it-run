# Pi-Bolt

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/opensec-git/Pi-Bolt, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pi-bolt

## Pinned environment

- Project commit: `956090824caa8c7fdd0b8d780aae552a2cde5510`
- Test commit: `956090824caa8c7fdd0b8d780aae552a2cde5510`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 28.5 to 28.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 28.5 | 3 | 3 | [run](https://argusic.com/run/6a85beb6-e2b9-4246-89a7-2a37921f6a5c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 in container, project requires >=22.19`
- 2 min: `Type error in packages/ai/src/providers/opencode-go.ts: missing google-generative-ai API support in data`
- `3 pre-existing test failures in resource-loader.test.ts (CWD-dependent paths)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
