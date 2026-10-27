# awesome-llm-services

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/av/awesome-llm-services, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/awesome-llm-services

## Pinned environment

- Project commit: `7c3dbd04d0d22031e330da7d338d8024fbf6773c`
- Test commit: `7c3dbd04d0d22031e330da7d338d8024fbf6773c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.3 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.2 | 8.3 | 2 | 2 | [run](https://argusic.com/run/c36ebcd4-b3d6-42d4-bf0a-992ad0cdc4cf) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Deno not pre-installed; needed for README generator`
- 1 min: `GitHub unauthenticated rate limit (60 req/hr) would stall generator for ~3600s per retry`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
