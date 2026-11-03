# guzzle

**Verdict: runs.** Argusic Score 94 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/guzzle/guzzle, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/guzzle

## Pinned environment

- Project commit: `93939470950a9b11e2e84204166ef5e048c55fe4`
- Test commit: `93939470950a9b11e2e84204166ef5e048c55fe4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 25.4 to 35.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 35.5 | 7 | 7 | [run](https://argusic.com/run/4e962675-e9e8-439f-86b4-78542661f014) |
| 2 | pass | 96 | 8 | 25.4 | 5 | 4 | [run](https://argusic.com/run/9cd1a6fe-8376-4dc8-b085-ab3186507844) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No PHP or Composer in container; downloaded static PHP 8.4.6 (bulk) and Composer 2.10.3`
- 2 min: `Circular dependency: guzzlehttp/test-server requires guzzlehttp/guzzle ^8.1 but root package had no version`
- 5 min: `Initial static PHP build (common/php-8.3.17) had libcurl without HTTP/2 support, causing 56 errors`
- 3 min: `StreamHandler 'Address not available' not in CONNECTION_ERRORS, causing 2 test failures`
- `PHP built-in test server on port 10000 unreliable in this shell; 51 HttplugIntegrationTest errors`
- `CurlFactory test: testStreamedUploadFailsFastOnChallengeRewind fails because this libcurl (8.13.0) lacks CURLOPT_SEEKFUNCTION, altering digest auth retry behavior`
- `Node.js test server background process management unreliable`

Attempt 2:

- 6 min: `PHP 7.4+ runtime not installed in container; no root access for apt`
- 2 min: `composer install failed: guzzlehttp/test-server requires guzzlehttp/guzzle ^8.1 but root package is a dev ref`
- 1 min: `ctype_digit() undefined: ctype.so not loaded in static PHP build`
- 2 min: `HttplugIntegrationTest errors: 51 connection failures to port 10000 and 8126 test servers`
- `StreamHandlerTest::testDoesNotLeakRequestUriCredentialsInConnectionErrorMessage errors and testAddsErrorToResponse fails: environment-specific connect behavior (localhost:123 yields RequestException instead of ConnectException)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
