# ffmpeg-skill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kajisho5/ffmpeg-skill, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ffmpeg-skill

## Pinned environment

- Project commit: `f6af42f25f9df42d11754f36c8b08f3ceb26a101`
- Test commit: `f6af42f25f9df42d11754f36c8b08f3ceb26a101`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 25.1 to 72.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 25.1 | 0 | 0 | [run](https://argusic.com/run/71a268b0-da2d-43f5-bca2-f87d71114d7e) |
| 2 | pass | 100 | 51 | 72.1 | 1 | 1 | [run](https://argusic.com/run/6e710c51-6a4a-4dd8-8fd8-534df6a3fa4e) |

## What was observed on a clean machine

Attempt 2:

- 24 min: `second full-suite run failed (exit 1) because previous runs left tests/out artifacts and MCP output locks, e.g. 'another run is writing out.mp4 right now' and cache_fail_out.mp4 existing; the suite asserts a clean output dir`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
