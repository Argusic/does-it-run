# testsprite-cli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TestSprite/testsprite-cli, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/testsprite-cli

## Pinned environment

- Project commit: `1921dcfe25d943ee94cf95e41af5ed87190ca793`
- Test commit: `1921dcfe25d943ee94cf95e41af5ed87190ca793`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 10.4 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/74282be7-7e7c-4547-9bab-297cc75705a4) |
| 2 | pass with mocks | 92 | 9 | 10.4 | 1 | 1 | [run](https://argusic.com/run/9cf63cc4-53e3-49eb-9b28-b50513239ca0) |

## What was observed on a clean machine

Attempt 2:

- 4 min: `7 ticker tests failed because NO_COLOR=1 leaked from the container env into ticker.ts's isNoColor() check, making TTY-mode tests enter NO_COLOR mode`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
