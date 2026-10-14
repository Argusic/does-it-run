# sharp

**Verdict: runs.** Argusic Score 98 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/code16/sharp, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/sharp

## Pinned environment

- Project commit: `1482e3753965de75bfe4f106d5c8467c5f77f74c`
- Test commit: `1482e3753965de75bfe4f106d5c8467c5f77f74c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 29.5 to 29.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 98 | 25 | 29.5 | 10 | 9 | [run](https://argusic.com/run/cc86e63a-631c-48ee-bbef-407ca9e6fb71) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `PHP not installed`
- 1 min: `Composer not installed`
- 1 min: `Security advisory blocked enshrined/svg-sanitize`
- 2 min: `Composer zip extension missing`
- 1 min: `PHP memory limit 128M too low for parallel tests`
- 5 min: `GD extension missing causing 63 test failures`
- 2 min: `Node 18 too old for Vite 8 which needs 20.19+`
- 1 min: `Rolldown native binding missing for Vite build`
- 2 min: `php artisan serve subprocess clears PHPRC and LD_LIBRARY_PATH`
- `npm test references jest which is not a dependency`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
