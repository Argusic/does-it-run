# skills

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/skills, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/18801799-dce4-4c4c-9b72-e2940b119c91

## Pinned environment

- Project commit: `23d0dac5f83f268166a17f0bc7dc6c73dc348a33`
- Test commit: `23d0dac5f83f268166a17f0bc7dc6c73dc348a33`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 0.5 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2.1 | 7.8 | 4 | 4 | [run](https://argusic.com/run/18801799-dce4-4c4c-9b72-e2940b119c91) |
| 2 | fail | 20 | n/a | 0.5 | 0 | 0 | [run](https://argusic.com/run/f59c20c5-c9b3-4c61-88c3-70e3e153d93b) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pnpm not available globally (no root); used npx pnpm instead`
- 1 min: `Node v18 < v22 requirement; harness runner works but vitest unit tests fail`
- `rolldown native binary missing: rolldown-binding.linux-x64-gnu.node not in pnpm store; vitest cannot start`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
