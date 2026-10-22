# prompt-cache

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/messkan/prompt-cache, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/prompt-cache

## Pinned environment

- Project commit: `9fc9025dd148400527d77342c0c8dbd8fa369470`
- Test commit: `9fc9025dd148400527d77342c0c8dbd8fa369470`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.5 to 16.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 16.5 | 3 | 3 | [run](https://argusic.com/run/939d5824-3418-4658-b804-769d8ea84948) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go 1.24 runtime not installed in container`
- 3 min: `BadgerDB Get() swallowed ErrKeyNotFound returning nil,nil instead of propagating error`
- 1 min: `BadgerDB tests expected error on missing key but storage returns nil,nil; TTL expiry test also expected error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
