# invobook

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Hasnayeen/invobook, licensed MIT, written in Blade.

Evidence and recordings: https://argusic.com/subject/invobook

## Pinned environment

- Project commit: `e5f666cef63543beffadfcc045f6af673408a02e`
- Test commit: `e5f666cef63543beffadfcc045f6af673408a02e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 8.4 to 9.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 9.2 | 7 | 7 | [run](https://argusic.com/run/5877154e-1114-4fd0-b221-d9d4e2ccf047) |
| 2 | pass with mocks | 92 | 6.5 | 8.4 | 4 | 4 | [run](https://argusic.com/run/4e74cf86-d433-459b-bfd0-4ab1d88b0f7c) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `PHP 8.x not installed in container`
- 2 min: `Composer not installed`
- 8 min: `Required PHP extensions (dom, intl, tokenizer, fileinfo, xmlreader, xmlwriter, simplexml, zip) missing`
- 3 min: `libzip shared library missing for zip extension`
- 5 min: `PDO SQLite driver not registering - undefined symbols`
- 5 min: `MySQL not available but project defaults to MySQL`
- 2 min: `post-autoload-dump composer script (package:discover) fails on config resolution but non-fatal`

Attempt 2:

- 5.5 min: `PHP runtime not installed in container`
- 0.2 min: `composer install failed during post-autoload-dump because APP_KEY was empty and 'config' class not found`
- 0.3 min: `Symfony polyfill-mbstring iconv_strrpos() error during HTTP requests via artisan serve`
- 0.5 min: `php8.3-zip.so from Ubuntu 24.04 requires libzip.so.4 with symbol zip_register_cancel_callback_with_state which libzip4 1.0.1 from Ubuntu 24.04 lacks`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
