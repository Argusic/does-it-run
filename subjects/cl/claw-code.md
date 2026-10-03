# claw-code

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ultraworkers/claw-code, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/claw-code

## Pinned environment

- Project commit: `08106b0c3771ef5b4a5aa176acccd460e88b7325`
- Test commit: `08106b0c3771ef5b4a5aa176acccd460e88b7325`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 4; wall time 4.9 to 9.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 9.9 | 1 | 1 | [run](https://argusic.com/run/28be8f91-6439-4633-9fb1-344e57922875) |
| 1 | pass | 100 | 2 | 4.9 | 0 | 0 | [run](https://argusic.com/run/e4339676-58f1-4783-bf4b-8341b4854738) |
| 2 | pass with mocks | 92 | 15 | 6.7 | 0 | 0 | [run](https://argusic.com/run/fb0a2cd4-89b7-4c1d-a895-bf88d7bf44d5) |
| 3 | pass with mocks | 92 | 2 | 5.9 | 0 | 0 | [run](https://argusic.com/run/f3036bd5-7183-464f-a215-e4457faee41b) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `10 clippy linting errors in claw-rag-service and runtime crates`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
