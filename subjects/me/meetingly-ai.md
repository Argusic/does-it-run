# meetingly-ai

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iskandaryv/meetingly-ai, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/meetingly-ai

## Pinned environment

- Project commit: `e55cc045e18ae426d67aaef4d524212ebb6abded`
- Test commit: `e55cc045e18ae426d67aaef4d524212ebb6abded`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.2 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 13 | 10.2 | 5 | 5 | [run](https://argusic.com/run/d9d4ea20-c05f-4872-98cd-23ceeabebb82) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `vitest/rolldown failed on Node 18: node:util has no styleText export`
- 2 min: `rolldown native binding missing after install (npm optional-deps bug)`
- 2 min: `Electron SUID sandbox helper not configured (no root in container)`
- 2 min: `Mock upstream for relay died (bad empty-body handling in my first mock on Node 18)`
- 3 min: `App chat smoke returned 401 Invalid app token against my mock relay`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
