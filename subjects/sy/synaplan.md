# synaplan

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/metadist/synaplan, licensed Apache-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/synaplan

## Pinned environment

- Project commit: `619349a25bb173c1b4a7f644591ac2c005ad2312`
- Test commit: `619349a25bb173c1b4a7f644591ac2c005ad2312`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 41.8 to 41.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 41.8 | 3 | 3 | [run](https://argusic.com/run/b7f5595b-2fa7-41f5-b99a-a21a0e8eb014) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18 is too old , project requires >= 24`
- 2 min: `Optional native bindings not installed (npm CI bug)`
- 8 min: `frontend/src/generated/api-schemas.ts not present (generated from OpenAPI spec at build time)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
