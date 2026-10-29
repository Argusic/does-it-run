# ecommerce-template

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MarcosCamara01/ecommerce-template, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ecommerce-template

## Pinned environment

- Project commit: `3971973750d293747969e57759252b8f1b298b0c`
- Test commit: `3971973750d293747969e57759252b8f1b298b0c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.8 to 13.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.25 | 13.8 | 1 | 1 | [run](https://argusic.com/run/a5775c28-d9ea-4a25-9c28-fc7640550c5f) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `create-validation.test.mjs fails: tsx --eval wraps .ts exports under .default key`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
