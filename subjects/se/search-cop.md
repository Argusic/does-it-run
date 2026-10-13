# search_cop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mrkamel/search_cop, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/search-cop

## Pinned environment

- Project commit: `0ac931010c2dc42e55116b841c050395460c3797`
- Test commit: `0ac931010c2dc42e55116b841c050395460c3797`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 7.2 | 5 | 5 | [run](https://argusic.com/run/89c6d079-8f49-4e19-9070-d57e2ace3c08) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `No Ruby runtime in container (ruby/gem/bundle absent) and no root apt access`
- 3 min: `gem install mysql2 failed: ld cannot find -lzstd (Ubuntu 24.04 libmysqlclient links libzstd)`
- 2 min: `gem build of mysql2 extension failed: static libz.a linked into a shared object (relocation error for z_errmsg)`
- 2 min: `DATABASE=postgres suite failed at enable_extension citext (non-superuser search_cop role)`
- 1 min: `Local PostgreSQL trial listened on port 55432 while test/database.yml hardcodes 127.0.0.1:5432 (Connection refused)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
