# runner

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yicheng47/runner, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/runner

## Pinned environment

- Project commit: `3d83d697f7176c0a3d62b047fe3a641ab7ae8249`
- Test commit: `3d83d697f7176c0a3d62b047fe3a641ab7ae8249`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.1 to 16.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 16.1 | 1 | 1 | [run](https://argusic.com/run/bdee6f35-9d96-4a7c-aed2-e8a76f955bd7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test stop_reaps_descendants_the_agent_left_behind failed because /bin/zsh is not installed in the container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
