# ShopifyAutoAuth

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AhmadHassan-BTed/ShopifyAutoAuth, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/shopifyautoauth

## Pinned environment

- Project commit: `af75a4e20b2eda5bc8cd973500e7b46fc79f0691`
- Test commit: `af75a4e20b2eda5bc8cd973500e7b46fc79f0691`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 0.9 to 1.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 1.3 | 0 | 0 | [run](https://argusic.com/run/ef3c39f3-3583-4de2-ada2-a95e7db41420) |
| 2 | pass | 100 | 2 | 0.9 | 0 | 0 | [run](https://argusic.com/run/d5abd810-271b-4c6b-8a63-3b6a71af1040) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
