# guzzle

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/guzzle/guzzle, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/guzzle

## Pinned environment

- Project commit: `93939470950a9b11e2e84204166ef5e048c55fe4`
- Test commit: `93939470950a9b11e2e84204166ef5e048c55fe4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 35.5 to 35.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 35.5 | 7 | 7 | [run](https://argusic.com/run/4e962675-e9e8-439f-86b4-78542661f014) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No PHP or Composer in container; downloaded static PHP 8.4.6 (bulk) and Composer 2.10.3`
- 2 min: `Circular dependency: guzzlehttp/test-server requires guzzlehttp/guzzle ^8.1 but root package had no version`
- 5 min: `Initial static PHP build (common/php-8.3.17) had libcurl without HTTP/2 support, causing 56 errors`
- 3 min: `StreamHandler 'Address not available' not in CONNECTION_ERRORS, causing 2 test failures`
- `PHP built-in test server on port 10000 unreliable in this shell; 51 HttplugIntegrationTest errors`
- `CurlFactory test: testStreamedUploadFailsFastOnChallengeRewind fails because this libcurl (8.13.0) lacks CURLOPT_SEEKFUNCTION, altering digest auth retry behavior`
- `Node.js test server background process management unreliable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
