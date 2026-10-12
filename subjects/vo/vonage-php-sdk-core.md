# vonage-php-sdk-core

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Vonage/vonage-php-sdk-core, licensed Apache-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/vonage-php-sdk-core

## Pinned environment

- Project commit: `9c6bc46e70451d2dc6c8243ba04dc34121878199`
- Test commit: `9c6bc46e70451d2dc6c8243ba04dc34121878199`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.9 to 3.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 3.9 | 2 | 2 | [run](https://argusic.com/run/76375507-b749-47f9-bb1d-f421615e057f) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Container had no php or composer (no root to apt-get); installed prebuilt static PHP 8.5.8 and Composer 2.10.3 into /tmp`
- 6 min: `composer test: 13 errors + 3 failures, TypeError Vonage\Client::setHttpClient(): Argument #1 must be Psr\Http\Client\ClientInterface, null given in src/Client.php:146`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
