# dotfiles

**Verdict: could not verify.** Argusic Score 45 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/driesvints/dotfiles, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/dotfiles

## Pinned environment

- Project commit: `0d7a71d7330540329f0bff995ee577bf432a4bc7`
- Test commit: `0d7a71d7330540329f0bff995ee577bf432a4bc7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 4.4 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 4.4 | 0 | 0 | [run](https://argusic.com/run/6bf2a689-5821-4049-88e9-29c3cc8bb4f0) |
| 2 | fail | 70 | 5 | 6.4 | 2 | 1 | [run](https://argusic.com/run/6d136c66-d45a-4895-8bb7-47252bfc1b55) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Zsh native modules (zle.so, parameter.so) missing from bundled zsh , oh-my-zsh shell integration degraded`
- 1 min: `SSH unavailable for git submodule , used HTTPS fallback for plugins/artisan`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
