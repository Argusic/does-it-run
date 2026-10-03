# xgplayer

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bytedance/xgplayer, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/xgplayer

## Pinned environment

- Project commit: `2c4e5f6c44af7a536b3b8c39c5f4f7567b08078e`
- Test commit: `2c4e5f6c44af7a536b3b8c39c5f4f7567b08078e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.5 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.1 | 7.5 | 2 | 2 | [run](https://argusic.com/run/481b9fa9-d147-4e6a-8c45-611b1136f9a4) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `FetchLoader._getRangeResponseMismatchReason had guard 'if (!this._rangeRequestMustReturn206)' preventing content-range validation when flag was falsy, causing test 'rejects range request when content-range and content-length do not match re`
- 2 min: `XhrLoader._getRangeResponseMismatchReason had same guard as fetch.js causing identical test failure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
