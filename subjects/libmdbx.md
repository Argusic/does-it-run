# libmdbx

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Mithril-mine/libmdbx, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/libmdbx

## Pinned environment

- Project commit: `7f84421879896670dd7e7233af16614490cf6ba4`
- Test commit: `7f84421879896670dd7e7233af16614490cf6ba4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.6 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 2.6 | 1 | 1 | [run](https://argusic.com/run/9d3fcb63-5c66-4f3d-8346-e01d234549ab) |
| 2 | pass | 100 | 2 | 11.5 | 1 | 1 | [run](https://argusic.com/run/684c35e4-0a7b-468d-b857-593ff0aec662) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `make check fails because it forces Ninja generator (cmake -G Ninja) but Ninja is not installed in the container`

Attempt 2:

- 2 min: `make check requires Ninja (cmake -G Ninja), which is not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
