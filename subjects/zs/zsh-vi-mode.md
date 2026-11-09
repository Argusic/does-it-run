# zsh-vi-mode

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jeffreytse/zsh-vi-mode, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/zsh-vi-mode

## Pinned environment

- Project commit: `91cafe4a09b6670cb8e761aa413e5f7b9e00816f`
- Test commit: `91cafe4a09b6670cb8e761aa413e5f7b9e00816f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.1 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 6.1 | 1 | 1 | [run](https://argusic.com/run/893d3ecc-e690-408b-a83c-35eb78fe098f) |
| 2 | pass | 100 | 36 | 14 | 5 | 5 | [run](https://argusic.com/run/8fdddaa8-18f0-4fd0-9d91-39cd5aa6583d) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `zsh was not installed in the container`
- 2 min: `ncurses development headers missing (libncurses-dev)`
- 1 min: `no controlling tty during configure`
- 1 min: `static ncurses .a files lacked -fPIC, shared module linking failed`
- 1 min: `zsh/regex module not linked (link=no in config.modules)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
