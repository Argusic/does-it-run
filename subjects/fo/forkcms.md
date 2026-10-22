# forkcms

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/forkcms/forkcms, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/forkcms

## Pinned environment

- Project commit: `0545b76bc67e0c6f53e057c4b2f64d218374a057`
- Test commit: `0545b76bc67e0c6f53e057c4b2f64d218374a057`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.1 to 23.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 23.1 | 5 | 5 | [run](https://argusic.com/run/e62a5c7c-25fb-4101-b17a-46d4129b6f68) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `PHP 8.4 not available - needed static PHP binary`
- 1 min: `composer.lock requires PHP <8.2, blocked install`
- 8 min: `No MySQL server available for tests requiring a database`
- 3 min: `PHP 8.4 changed preg_match lookbehind assertion - test failure`
- `Profiles ModelTest::testInsertingProfileGroup fails - PDO returns ints not strings (PHP 8.4)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
