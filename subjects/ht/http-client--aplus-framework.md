# http-client

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aplus-framework/http-client, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/run/0b3023dc-6469-4783-bea0-98c44b724e0e

## Pinned environment

- Project commit: `11c54b718dcd6a364bb0bdea4acb57cdbce96727`
- Test commit: `11c54b718dcd6a364bb0bdea4acb57cdbce96727`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.7 to 13.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 13.7 | 4 | 4 | [run](https://argusic.com/run/0b3023dc-6469-4783-bea0-98c44b724e0e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP 8.3 not installed in container`
- 3 min: `Missing required PHP extensions (curl, phar, fileinfo, iconv, mbstring, intl, xml, xdebug, dom, simplexml, xmlwriter, tokenizer)`
- 1 min: `xsl.so and zip.so failed to load (missing system libraries libxslt.so.1 and libzip.so.4)`
- 2 min: `Composer install failed due to missing zip/unzip support`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
