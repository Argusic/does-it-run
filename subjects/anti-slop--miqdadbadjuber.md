# anti-slop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/miqdadbadjuber/anti-slop, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/run/3595bcb3-e4d6-4cf8-931a-0780eacb376e

## Pinned environment

- Project commit: `91f12ec67e9de6043cfd93b846404986ba73c3f4`
- Test commit: `91f12ec67e9de6043cfd93b846404986ba73c3f4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11 to 11 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 11 | 1 | 1 | [run](https://argusic.com/run/3595bcb3-e4d6-4cf8-931a-0780eacb376e) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `@clack/prompts@1.7.0 uses import { styleText } from 'node:util' which requires Node >= 20.12.0, but container has Node 18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
