# powerlevel10k

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/romkatv/powerlevel10k, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/powerlevel10k

## Pinned environment

- Project commit: `7ddd1b2715c3844275214347a3572ac1fdd6dc39`
- Test commit: `7ddd1b2715c3844275214347a3572ac1fdd6dc39`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.3 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 4.3 | 2 | 2 | [run](https://argusic.com/run/71b683b5-5c12-4b06-b7c8-555b2f881c54) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Zsh not installed in container`
- 2 min: `gitstatusd binary not pre-built and system libgit2 API incompatible`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
