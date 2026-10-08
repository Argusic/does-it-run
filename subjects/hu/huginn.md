# huginn

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/huginn/huginn, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/huginn

## Pinned environment

- Project commit: `5658f26d4c176e3b6052dc0a6f400f5a45a6ec83`
- Test commit: `5658f26d4c176e3b6052dc0a6f400f5a45a6ec83`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11 to 11 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 27 | 11 | 3 | 3 | [run](https://argusic.com/run/730f7920-64de-4d1e-a15d-6b237ca7f520) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `mysql2 native extension failed - no MySQL client headers`
- 1 min: `fontawesome CSS asset missing on home page`
- 1 min: `URL polyfill not found for JavaScriptAgent`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
