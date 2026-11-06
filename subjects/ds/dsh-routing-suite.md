# dsh-routing-suite

**Verdict: runs.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yjh051108/dsh-routing-suite, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dsh-routing-suite

## Pinned environment

- Project commit: `195273352f23bff7f9023ebe2ec0cdbdf9c98f10`
- Test commit: `195273352f23bff7f9023ebe2ec0cdbdf9c98f10`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 8.9 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6.2 | 8.9 | 2 | 2 | [run](https://argusic.com/run/feff23a9-5155-43ba-bdc5-4879eba94c32) |
| 2 | fail | 50 | 30 | 11.7 | 6 | 6 | [run](https://argusic.com/run/bd0bf2b9-2a88-4221-bfe1-61dc55d33613) |

## What was observed on a clean machine

Attempt 1:

- 3.5 min: `System Node.js v18.19.1 too old (project requires >=22); injector build (tsdown/rolldown) fails without native binding optional deps`
- 2.5 min: `Root package test 2 (pack --dry-run) fixture missing injector/scripts/prepare.mjs, and npm 10+ interleaves prepare stdout with JSON output`

Attempt 2:

- 2 min: `confirm.test.mjs imports ../src/confirm.js but source in same directory`
- 2 min: `plan-tree.test.mjs imports ../src/plan-tree.js but source in same directory`
- 2 min: `root-package-prepare.test.mjs pack test fails because npm runs prepare even with --ignore-scripts`
- 5 min: `dsh plugin add requires pnpm (not installed)`
- 3 min: `System Node.js v18.19.1 < required >=22`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
