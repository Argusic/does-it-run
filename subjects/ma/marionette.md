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
- Valid runs: 2; wall time 3.3 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.3 | 1 | 1 | [run](https://argusic.com/run/0ba85299-a5d1-48c5-a293-3f46be0b8dc5) |
| 2 | pass | 100 | 5 | 3.3 | 3 | 3 | [run](https://argusic.com/run/1cc78839-ee0d-4b0c-b087-c5a267011a6b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Container had Node v18.19.1 but project requires ^22.22.2 || >=24.15.0`

Attempt 2:

- 3 min: `System Node is v18.19.1, below the engines minimum (^22.22.2 || >=24.15.0) and below npm@11.17.0 support; npm 9.2.0 warned about it`
- `Probe importing 'jsdom' from /tmp failed with ERR_MODULE_NOT_FOUND because /tmp is outside the repo module graph`
- 1 min: `Dist-ESM probe hit TypeError 'app.prepare is not a function' (Application has no prepare method in 5.0.0)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
