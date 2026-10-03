# google-play-scraper

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/facundoolano/google-play-scraper, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/google-play-scraper

## Pinned environment

- Project commit: `20359f62469cfec14b9718c4cf16aa1dfd8a2864`
- Test commit: `20359f62469cfec14b9718c4cf16aa1dfd8a2864`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.1 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 8.1 | 2 | 2 | [run](https://argusic.com/run/74ddee63-69f9-4ea1-b680-4696de27b210) |

## What was observed on a clean machine

Attempt 1:

- `mocha@12.0.0 requires Node.js 20+, container has 18.19.1`
- 1 min: `test failure: assertValidUrl(app.video) on undefined , Google Play no longer serves a trailer for Clash of Clans`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
