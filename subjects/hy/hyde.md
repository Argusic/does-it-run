# hyde

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hydephp/hyde, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/hyde

## Pinned environment

- Project commit: `ede2acbc844e8b44464e03d49bc55192be0c57c5`
- Test commit: `ede2acbc844e8b44464e03d49bc55192be0c57c5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.1 to 12.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12.1 | 6 | 6 | [run](https://argusic.com/run/c3a9d540-a32d-42ad-8561-9bc863969475) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No PHP binary found in container`
- 1 min: `Composer not available`
- 4 min: `Missing test base classes (TestCase.php, UnitTestCase.php)`
- 2 min: `PHPUnit 12 incompatible with Laravel Zero 11 ErrorHandler::enable() signature`
- 1 min: `Missing Mockery for Laravel console testing`
- 2 min: `Facade root not set in UnitTestCase resetKernel()`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
