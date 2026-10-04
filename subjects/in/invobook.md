# invobook

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Hasnayeen/invobook, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/invobook

## Pinned environment

- Project commit: `e5f666cef63543beffadfcc045f6af673408a02e`
- Test commit: `e5f666cef63543beffadfcc045f6af673408a02e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.2 to 9.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 9.2 | 7 | 7 | [run](https://argusic.com/run/5877154e-1114-4fd0-b221-d9d4e2ccf047) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `PHP 8.x not installed in container`
- 2 min: `Composer not installed`
- 8 min: `Required PHP extensions (dom, intl, tokenizer, fileinfo, xmlreader, xmlwriter, simplexml, zip) missing`
- 3 min: `libzip shared library missing for zip extension`
- 5 min: `PDO SQLite driver not registering - undefined symbols`
- 5 min: `MySQL not available but project defaults to MySQL`
- 2 min: `post-autoload-dump composer script (package:discover) fails on config resolution but non-fatal`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
