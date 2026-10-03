# baoyu-design

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JimLiu/baoyu-design, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/baoyu-design

## Pinned environment

- Project commit: `6530033592bf7fa58bc1a5a2a2ad278da45213a9`
- Test commit: `6530033592bf7fa58bc1a5a2a2ad278da45213a9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.5 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0 | 5.5 | 1 | 1 | [run](https://argusic.com/run/9069b45a-6140-414e-bf77-dca7df0fe360) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `package.json test script used single quotes around glob pattern, preventing shell expansion - npm test failed with 'Could not find' error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
