# shopper

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shopperlabs/shopper, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/shopper

## Pinned environment

- Project commit: `86da81306a7f3b0f981ccd196182fb15481dea6c`
- Test commit: `86da81306a7f3b0f981ccd196182fb15481dea6c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 59.6 to 59.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 59.6 | 9 | 9 | [run](https://argusic.com/run/8ed0bcb4-1068-4dc9-b217-7076693cd97c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP 8.3 binary not available in container`
- 2 min: `Required PHP extensions (phar, iconv, intl, mbstring, tokenizer, fileinfo, curl, dom, exif, soap, xml, sqlite3, pdo_sqlite, zip, gd) missing`
- 1 min: `Shared library dependencies (libgd.so.3, libzip.so.4) not found`
- 1 min: `Composer binary not available`
- 2 min: `Lock file required PHP >=8.4.1 but only PHP 8.3 available`
- 1 min: `PDO SQLite driver not loaded, causing could not find driver error`
- `Memory limit exhausted (128M default) during tests`
- 1 min: `GD extension could not load without libgd`
- `npm build has Node.js version incompatibility (node 18 vs 20 required)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
