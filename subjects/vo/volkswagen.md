# volkswagen

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/auchenberg/volkswagen, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/volkswagen

## Pinned environment

- Project commit: `ae379b4459ee4dd71b4783246b99f6a3135fdc4b`
- Test commit: `ae379b4459ee4dd71b4783246b99f6a3135fdc4b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.6 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.12 | 13.6 | 2 | 2 | [run](https://argusic.com/run/4fb70f30-e0da-40c5-a020-de20d509ae5e) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `test/chai.js crashed on assert.include() with no arguments because chai v4.5.0 adds methods not stubbed by the defeat device (isOk, include, lengthOf, match, propertyNotVal, etc.)`
- 2 min: `test/chai.js used deprecated chai assert method names (assert.propertyNotVal, assert.deepProperty, assert.notDeepProperty, assert.deepPropertyNotVal) that no longer exist in chai v4.5.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
