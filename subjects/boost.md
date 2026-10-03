# boost

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/laravel/boost, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/boost

## Pinned environment

- Project commit: `c0b668cd2d5e565507b5bd05ee71f8e322c660e7`
- Test commit: `c0b668cd2d5e565507b5bd05ee71f8e322c660e7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.6 to 7.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 7.6 | 2 | 2 | [run](https://argusic.com/run/50a41fcc-6713-47ed-8487-5ba0622fafa1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP and Composer not pre-installed in container`
- 1 min: `Static PHP binary memory limit (128M) too low for ArchTest when run in full suite`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
