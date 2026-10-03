# PhpSpreadsheet

**Verdict: runs.** Argusic Score 73.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PHPOffice/PhpSpreadsheet, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/phpspreadsheet

## Pinned environment

- Project commit: `d6bd070cb0c53a5ac488666f5e43513bb5117978`
- Test commit: `d6bd070cb0c53a5ac488666f5e43513bb5117978`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 15.1 to 46.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 15.1 | 0 | 0 | [run](https://argusic.com/run/b47b1735-d71d-410f-a0d2-5ab047c8009e) |
| 2 | pass | 100 | 35 | 36.3 | 5 | 5 | [run](https://argusic.com/run/7b0cb398-82c2-4481-911e-48c9c16751b6) |
| 3 | pass | 100 | 37 | 46.4 | 7 | 7 | [run](https://argusic.com/run/fb4fd8da-cd27-4d93-98fd-128531250d5b) |

## What was observed on a clean machine

Attempt 2:

- 12 min: `PHP and Composer not found on system`
- 5 min: `Phar extension missing (needed by Composer)`
- 5 min: `Missing extensions: mbstring, dom, simplexml, xml, xmlreader, xmlwriter, curl, intl`
- 3 min: `Missing system libraries for gd and zip extensions (libgd.so.3, libzip.so.4)`
- 10 min: `Composer install of 82 packages timed out on first attempts (git clone mirror for large repos)`

Attempt 3:

- 1 min: `PHP not installed in container`
- 1 min: `Composer not installed in container`
- 3 min: `ext-intl missing in common static PHP build`
- 1 min: `Composer lock requires ext-intl for full install`
- 15 min: `20 test failures: 13 locale-related due to musl libc limitation (localeconv returns '.' regardless of setlocale)`
- 2 min: `7 network-dependent test failures (URL image downloads blocked by container proxy)`
- 10 min: `glibc locale charmaps missing for localedef`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
