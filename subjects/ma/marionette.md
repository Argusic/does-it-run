# marionette

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/marionettejs/marionette, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/marionette

## Pinned environment

- Project commit: `0f2284ad4bbfe8c82ce82714471697a68c2acaeb`
- Test commit: `0f2284ad4bbfe8c82ce82714471697a68c2acaeb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.3 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.3 | 1 | 1 | [run](https://argusic.com/run/0ba85299-a5d1-48c5-a293-3f46be0b8dc5) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Container had Node v18.19.1 but project requires ^22.22.2 || >=24.15.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
