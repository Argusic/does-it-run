# aws-codebuild-run-build

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aws-actions/aws-codebuild-run-build, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/aws-codebuild-run-build

## Pinned environment

- Project commit: `85cb4d9a6537e8456d6845d7cdf031a005181c3b`
- Test commit: `85cb4d9a6537e8456d6845d7cdf031a005181c3b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.1 to 1.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 1.1 | 1 | 1 | [run](https://argusic.com/run/68289e51-2f3f-4b85-a493-c8b31427e70d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `@actions/github v8.0.1 is ESM-only but the project uses CommonJS require(), causing ERR_REQUIRE_ESM at startup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
