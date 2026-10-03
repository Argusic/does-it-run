# blackcandy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/blackcandy-org/blackcandy, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/blackcandy

## Pinned environment

- Project commit: `6c36030c60c6de223058e7beeca92582b173efaf`
- Test commit: `6c36030c60c6de223058e7beeca92582b173efaf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 16 to 50.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 42 | 50.6 | 7 | 7 | [run](https://argusic.com/run/a4adb99c-b7d2-4709-99f8-3d7aa3348653) |
| 2 | pass | 100 | 30 | 42.3 | 5 | 5 | [run](https://argusic.com/run/75579ee7-3ec8-4b76-9fe0-73924c978b10) |
| 3 | pass | 100 | 14 | 16 | 3 | 3 | [run](https://argusic.com/run/dc771b56-da3e-4998-a3f4-bed1c91792b5) |

## What was observed on a clean machine

Attempt 1:

- 7 min: `Ruby 4.0.2 not found in container - no Ruby runtime at all`
- 5 min: `zlib extension not built - required by bundler`
- 7 min: `psych (YAML parser) extension not built - required by rubygems`
- 8 min: `pg gem requires libpq client library`
- 1 min: `psych version mismatch (lockfile requires 5.4.0, bundled 5.3.1)`
- 8 min: `libvips.so.42 and transitive dependencies missing for ruby-vips`
- `inotify instance limit reached during parallel tests`

Attempt 2:

- 10 min: `Ruby 4.0.7 not installed in container (missing Ruby entirely)`
- 2 min: `Node.js was v18.19.1 but project requires ^20.17.0 (specified 20.11.0 in .node-version)`
- 3 min: `pg gem (optional PostgreSQL driver) failed to compile due to missing libpq-dev`
- 7 min: `libvips.so.42 not found at runtime (missing library and all transitive dependencies)`
- 5 min: `One test failed due to missing libvips dependencies , MediaSyncAllJobTest#test_should_change_syncing_status`

Attempt 3:

- 7 min: `Ruby 4.0.2 not installed in container`
- 3 min: `pg gem native extension failed (libpq-dev headers missing)`
- 2 min: `libvips.so.42 missing causing test failure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
