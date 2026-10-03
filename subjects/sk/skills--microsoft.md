# skills

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/skills, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/18801799-dce4-4c4c-9b72-e2940b119c91

## Pinned environment

- Project commit: `23d0dac5f83f268166a17f0bc7dc6c73dc348a33`
- Test commit: `23d0dac5f83f268166a17f0bc7dc6c73dc348a33`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.8 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2.1 | 7.8 | 4 | 4 | [run](https://argusic.com/run/18801799-dce4-4c4c-9b72-e2940b119c91) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pnpm not available globally (no root); used npx pnpm instead`
- 1 min: `Node v18 < v22 requirement; harness runner works but vitest unit tests fail`
- `rolldown native binary missing: rolldown-binding.linux-x64-gnu.node not in pnpm store; vitest cannot start`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
