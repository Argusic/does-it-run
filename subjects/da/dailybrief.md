# DailyBrief

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/leiting-eric/DailyBrief, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dailybrief

## Pinned environment

- Project commit: `75e24a62e11c75453d918d2e8eeab51737d088e0`
- Test commit: `75e24a62e11c75453d918d2e8eeab51737d088e0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 33.9 to 33.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2.1 | 33.9 | 3 | 3 | [run](https://argusic.com/run/72649c9a-e546-4ed1-9b03-836662d2c32e) |

## What was observed on a clean machine

Attempt 1:

- 1.2 min: `Node.js 18 too old , cheerio + undici require >=20.18.1`
- 2.8 min: `No LLM credentials available , all 6 backends need an API key`
- 0.5 min: `Mock response selector matched GH enrichment before digest because digest systemPrompt mentions 'GitHub Trending' in rules`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
