# google-this

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LuanRT/google-this, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/google-this

## Pinned environment

- Project commit: `7e422b302fdded39562e8d5d1cdcfda25d06ea1f`
- Test commit: `7e422b302fdded39562e8d5d1cdcfda25d06ea1f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 33.2 to 33.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 33.2 | 3 | 3 | [run](https://argusic.com/run/d2eb800e-fdec-4971-863b-0e7e67d28b48) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm install nock v15 fails on node v18 (requires >=22)`
- 2 min: `search test fails because Google blocks real scraped requests`
- 2 min: `image test fails because Google blocks batch execute API`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
