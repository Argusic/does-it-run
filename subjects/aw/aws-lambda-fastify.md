# aws-lambda-fastify

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fastify/aws-lambda-fastify, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/aws-lambda-fastify

## Pinned environment

- Project commit: `402c265f911b18918af5d37452c0ff3d8b300a8a`
- Test commit: `402c265f911b18918af5d37452c0ff3d8b300a8a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4 to 4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 4 | 2 | 2 | [run](https://argusic.com/run/2424101c-c8f3-47d7-babd-12dd3833befa) |

## What was observed on a clean machine

Attempt 1:

- 18 min: `require() of ES Module cookie/dist/index.js from light-my-request/lib/cookies.js not supported`
- 8 min: `POST with base64 encoding test got 500 because multiValueHeaders array was assigned raw to header, causing Fastify inject to serialize with comma-space instead of comma`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
