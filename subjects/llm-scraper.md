# llm-scraper

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mishushakov/llm-scraper, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/llm-scraper

## Pinned environment

- Project commit: `2b43d999a17eac040f7cc315fc21dd526870564f`
- Test commit: `2b43d999a17eac040f7cc315fc21dd526870564f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 23.9 to 23.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 23.9 | 2 | 2 | [run](https://argusic.com/run/9cb495bc-81b4-49a2-b8c1-5d59c6a77d2b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `vitest 4.x requires Node 20+ (container has Node 18.19.1)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
