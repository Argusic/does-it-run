# lin-cms-vue

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/logamee/lin-cms-vue, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/lin-cms-vue

## Pinned environment

- Project commit: `16d3588825409d0ba678db0d2069cf50160342bd`
- Test commit: `16d3588825409d0ba678db0d2069cf50160342bd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.7 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 7.7 | 2 | 2 | [run](https://argusic.com/run/aacd61c4-39be-405a-a1cb-ec421b798107) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `jest.config.js referenced 'vue-jest' which is not available; @vue/vue3-jest needed for Vue 3`
- 2 min: `Presence of yarn.lock triggers mandatory yarn check during npm run serve; yarn is not installed and cannot be installed (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
