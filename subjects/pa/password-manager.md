# Password-Manager

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eusonlito/Password-Manager, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/password-manager

## Pinned environment

- Project commit: `ba8268a6f0cc2a90b142bb76a01dfa19481fc11f`
- Test commit: `ba8268a6f0cc2a90b142bb76a01dfa19481fc11f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 17.8 to 31.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 31.1 | 0 | 0 | [run](https://argusic.com/run/2c3750db-c882-4fa4-bf58-3333bfb23f24) |
| 2 | pass | 100 | 12 | 17.8 | 5 | 5 | [run](https://argusic.com/run/95cca5a8-501f-45eb-8f7b-7ff74ebf3264) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `No PHP binary in container`
- 5 min: `Composer platform conflict: vimeo/psalm requires PHP <= 8.3`
- 1 min: `SESSION_COOKIE env var missing causing TypeError in StartSession middleware`
- 1 min: `public/storage was a directory instead of symlink`
- 2 min: `Google Image Search scraping broken (regex no longer matches Google page)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
