# tuliprox

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/euzu/tuliprox, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/tuliprox

## Pinned environment

- Project commit: `cfc78fd64a22fea7a607e8f9217fc4fa5f66269e`
- Test commit: `cfc78fd64a22fea7a607e8f9217fc4fa5f66269e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19.9 to 19.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 19.9 | 5 | 5 | [run](https://argusic.com/run/c4d5b006-f7ba-45a4-a5b2-5a9d106ea2bd) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not installed`
- 3 min: `Sample config.yml had metadata.path and metadata.tmdb fields that do not exist in LibraryMetadataConfigDto`
- 1 min: `TULIPROX_PROXY_REWRITE_SECRET env var not set in sample config`
- 1 min: `Scan directories /media/movies and /media/tvshows in sample config did not exist`
- 1 min: `Web root directory did not exist for server mode`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
