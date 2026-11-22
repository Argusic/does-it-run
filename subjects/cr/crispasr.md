# CrispASR

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CrispStrobe/CrispASR, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/crispasr

## Pinned environment

- Project commit: `6b78932d09765406ba0e0154d95bc6289246ceee`
- Test commit: `6b78932d09765406ba0e0154d95bc6289246ceee`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 21.1 to 36.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 36 | 36.1 | 0 | 0 | [run](https://argusic.com/run/856d0143-3912-4000-bd4a-844dd79b3c2c) |
| 2 | pass | 100 | 21 | 21.1 | 1 | 1 | [run](https://argusic.com/run/148ae623-7fba-41b7-a8ca-df19cbd09339) |

## What was observed on a clean machine

Attempt 2:

- `test-c2pa-js-unit fails: Node.js v18.19.1 lacks crypto.randomUUID()`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
