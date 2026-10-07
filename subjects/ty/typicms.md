# typicms

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/typicms/typicms, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/typicms

## Pinned environment

- Project commit: `d12777b241fe73e68b7741129787dff8032581d2`
- Test commit: `d12777b241fe73e68b7741129787dff8032581d2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.2 to 24.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 24.2 | 5 | 5 | [run](https://argusic.com/run/60a0e268-1fdc-4959-be32-a7b7ecbf61e5) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No PHP or Composer available in container`
- 1 min: `No MySQL/PostgreSQL available`
- 1 min: `No Redis available for session/cache`
- 2 min: `Missing canonicalUrl() helper function in app/helpers.php`
- `28 vendor unit tests fail due to Pest/Laravel integration configuration for vendor directories`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
