# lithium

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/matt-42/lithium, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/lithium

## Pinned environment

- Project commit: `ac3fe63721b3c91b7fc6a477156c588c6fa38d82`
- Test commit: `ac3fe63721b3c91b7fc6a477156c588c6fa38d82`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 27.6 to 27.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 58 | 27.6 | 7 | 7 | [run](https://argusic.com/run/0fbcfccc-ecbc-4c93-be34-201f44d8187f) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `install.sh uses bash-specific [[ syntax, fails with /bin/sh`
- 15 min: `Missing Boost headers and libboost-context-dev (not installed in container)`
- 10 min: `Missing CURL, SQLite3, PostgreSQL, MariaDB dev packages`
- 3 min: `libmariadb.a needs OpenSSL symbols after it in link order`
- 8 min: `libmariadb.a also needs -lz (compress2/uncompress)`
- 5 min: `CURL::libcurl imported target had no IMPORTED_LOCATION with shared library, causing CURL::libcurl-NOTFOUND in build.make`
- 10 min: `5 tests fail: mysql_test, pgsql_test, orm_test, crud, sql_authentication (require live MySQL/PostgreSQL servers)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
