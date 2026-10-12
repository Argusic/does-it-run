# wikiman

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/filiparag/wikiman, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/wikiman

## Pinned environment

- Project commit: `353e165bf95cd1237e6bdf7590a1cbf1001c7a70`
- Test commit: `353e165bf95cd1237e6bdf7590a1cbf1001c7a70`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.2 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 14.2 | 4 | 4 | [run](https://argusic.com/run/d266dcd5-a0f1-4299-919e-97aa1c8ebd58) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `container had no man-db man binary (stub printed 'system minimized') and no fzf/rg/w3m/parallel/gawk`
- 4 min: `mawk 1.3.4 crashes with 'REcompile() - panic' on gentoo source regex, making the default full search emit a crash line`
- 2 min: `user-install layout mismatch: app computes ~/.local/share/share (build prefix $HOME/.local) and ~/.local/bin/wikiman symlink needed`
- 2 min: `initial mock wiki trees for tldr/arch/fbsd/gentoo/devdocs did not match source-module directory conventions, producing no results or malformed rows`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
