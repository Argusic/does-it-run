# Understand-Anything

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Egonex-AI/Understand-Anything, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/understand-anything

## Pinned environment

- Project commit: `ba450c43425f3de6d43daf76526950ad8ca93536`
- Test commit: `ba450c43425f3de6d43daf76526950ad8ca93536`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 7.8 to 17.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 17.4 | 1 | 1 | [run](https://argusic.com/run/6b4ff430-05b5-4e81-8d5f-e95c671f8bc3) |
| 2 | pass | 100 | 27 | 10 | 2 | 2 | [run](https://argusic.com/run/442af62c-a0b0-44e2-8a57-36b6a8ba2f4a) |
| 3 | pass with mocks | 92 | 12 | 7.8 | 1 | 1 | [run](https://argusic.com/run/6cceddfe-e2db-444d-af4c-6491d2d6fe61) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing @tailwindcss/oxide native binding for linux-x64-gnu platform`

Attempt 2:

- 2 min: `pnpm not available in PATH`
- 2 min: `@tailwindcss/oxide-linux-x64-gnu optional native binary missing from pnpm install (known pnpm optional-dependency issue)`

Attempt 3:

- 5 min: `Missing @tailwindcss/oxide-linux-x64-gnu native binding in pnpm isolated store; dashboard build and dashboard tests failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
