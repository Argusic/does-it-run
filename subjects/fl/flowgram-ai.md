# flowgram.ai

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bytedance/flowgram.ai, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/flowgram-ai

## Pinned environment

- Project commit: `ba1a9630f80263a196d31993cd85fd1c873d9ddd`
- Test commit: `ba1a9630f80263a196d31993cd85fd1c873d9ddd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.4 to 15.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 15.4 | 1 | 1 | [run](https://argusic.com/run/b5eaab9f-f472-4a11-9be9-f530aabfa02d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 does not satisfy required range >=18.20.3 <19.0.0 || >=20.14.0 <23.0.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
