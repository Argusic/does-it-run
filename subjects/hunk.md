# hunk

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/modem-dev/hunk, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/hunk

## Pinned environment

- Project commit: `aa23ba29ae233a480b1b3c2c20c1c25018246ee6`
- Test commit: `aa23ba29ae233a480b1b3c2c20c1c25018246ee6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 36.8 to 36.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 3 | 36.8 | 1 | 0 | [run](https://argusic.com/run/0d4dbe81-6ad7-49f5-a7a8-5abc81c9e0f3) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `canonical changelog versioning test fails - @changesets/cli@2.31.0 requires Node.js 22+ due to ESM/CJS human-id incompatibility`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
