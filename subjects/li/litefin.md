# litefin

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MoazSalem/litefin, licensed MPL-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/litefin

## Pinned environment

- Project commit: `0719489eb5466978967210861c1720ec91e7c198`
- Test commit: `0719489eb5466978967210861c1720ec91e7c198`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.6 to 15.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.2 | 15.6 | 2 | 2 | [run](https://argusic.com/run/632d682c-a383-44bb-b769-628d5ce5d2f2) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `tests/AudioChannelSettings.test.js: ReferenceError: navigator is not defined at WebOSAdapter._detectPlatform`
- 1 min: `tests/SubtitleFormatting.test.js: en-US.json locale file not found (case mismatch)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
