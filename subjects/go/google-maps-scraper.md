# google-maps-scraper

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gosom/google-maps-scraper, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/google-maps-scraper

## Pinned environment

- Project commit: `d0b51bcf3cd56d9a3f71e049cb6e226554e24162`
- Test commit: `d0b51bcf3cd56d9a3f71e049cb6e226554e24162`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 5.9 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 3 | 5.9 | 1 | 1 | [run](https://argusic.com/run/a278e8c4-1f7b-4359-8516-70e7cb9ecc6c) |
| 2 | pass with mocks | 92 | 1.5 | 6.1 | 0 | 0 | [run](https://argusic.com/run/ccee3d9b-aaae-4b31-8c25-242c7e0acf2d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go binary not found on system PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
