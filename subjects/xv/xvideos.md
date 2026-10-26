# xvideos

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rodrigogs/xvideos, licensed BSD-3-Clause, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/xvideos

## Pinned environment

- Project commit: `f6cfb6fbe712df1c32f29ab809c0d63127e12b4f`
- Test commit: `f6cfb6fbe712df1c32f29ab809c0d63127e12b4f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.6 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 4.6 | 3 | 3 | [run](https://argusic.com/run/ab1888c2-bccb-4767-8bf7-1653d8cdbe7e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 is too old (requires >=20.18.1) , vitest/rolldown native binding fails with 'styleText' import error`
- `Integration test 'loads verified list' fails , https://www.xvideos.com/verified/videos/1 returns HTTP 404`
- `3 additional integration tests fail (search navigation, detail, batch detail) , same root cause: live xvideos.com has changed URL patterns.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
