# cheat-on-content

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/XBuilderLAB/cheat-on-content, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/cheat-on-content

## Pinned environment

- Project commit: `d6b737bf79c1249b1848f8d1cccc0b248d513c56`
- Test commit: `d6b737bf79c1249b1848f8d1cccc0b248d513c56`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 2.9 to 4.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4.15 | 4.7 | 0 | 0 | [run](https://argusic.com/run/acf3f96c-d63b-40c7-bd51-69d04e4ec9e2) |
| 2 | pass | 100 | 2 | 2.9 | 2 | 2 | [run](https://argusic.com/run/abd9b69a-6fb2-4429-8b3b-21a8f7c4bc44) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Missing Python deps for adapters (httpx, requests, rapidfuzz)`
- `playwright not available for douyin/linkedin/wechat/weibo adapters`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
