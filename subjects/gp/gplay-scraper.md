# gplay-scraper

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Mohammedcha/gplay-scraper, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/gplay-scraper

## Pinned environment

- Project commit: `304dcd3d3546678dc386b412e1ec7c656d416459`
- Test commit: `304dcd3d3546678dc386b412e1ec7c656d416459`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.5 to 4.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.17 | 4.5 | 1 | 1 | [run](https://argusic.com/run/b3982116-ba2b-481b-b421-4ac9e77a8e80) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `tls_client client_identifier 'chrome112' is invalid; library expects 'chrome_112'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
