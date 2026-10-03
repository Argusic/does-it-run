# serverless-express

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CodeGenieApp/serverless-express, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/serverless-express

## Pinned environment

- Project commit: `4205db8998b31f4ceef1185c248c2d651d538cb0`
- Test commit: `4205db8998b31f4ceef1185c248c2d651d538cb0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.3 to 2.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 8 | 2.3 | 2 | 1 | [run](https://argusic.com/run/18cbf479-efe6-44c7-8f78-04737b6da68f) |

## What was observed on a clean machine

Attempt 1:

- `npm WARN EBADENGINE undici@7.24.7 requires node>=20.18.1, current v18.19.1; unicorn-magic@0.4.0 requires node>=20`
- `Console URIError logged during integration tests (expected error-path coverage, all test assertions passed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
