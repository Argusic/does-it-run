# mapwarper

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/timwaters/mapwarper, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/mapwarper

## Pinned environment

- Project commit: `1d56d8ea681a30bbde89033b4abab7a0ebf462ad`
- Test commit: `1d56d8ea681a30bbde89033b4abab7a0ebf462ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 36.5 to 36.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 36.5 | 14 | 14 | [run](https://argusic.com/run/23426acc-5603-4147-9fff-2e10c62062da) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Ruby 2.4.0 not installed in container`
- 5 min: `OpenSSL build failed: zlib.h not found`
- 5 min: `pg gem: libpq-fe.h not found`
- 8 min: `PostgreSQL server not available`
- 5 min: `PostGIS extension not loadable`
- 3 min: `PostGIS library missing dependencies`
- 1 min: `Devise secret_key not set`
- `secrets.yml missing`
- 3 min: `Import metadata content_type validation failed (Paperclip needs file command)`
- 2 min: `GDAL tools missing`
- 5 min: `GDAL binaries missing shared libraries`
- 2 min: `libgdal.so was a 35KB stub from libgdal-dev`
- 3 min: `PROJ: Cannot find proj.db`
- 1 min: `import_maps_sftp_path not writable (/home/sftpuser)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
