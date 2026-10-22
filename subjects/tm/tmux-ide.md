# tmux-ide

**Verdict: runs.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wavyrai/tmux-ide, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tmux-ide

## Pinned environment

- Project commit: `3237d0edc4e1e498f9a539c6b8943071a33da91a`
- Test commit: `3237d0edc4e1e498f9a539c6b8943071a33da91a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 10.5 to 37.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 10.5 | 0 | 0 | [run](https://argusic.com/run/d4f4405a-95e2-4cc0-927e-d207df1fa184) |
| 2 | pass | 92 | 37 | 37.4 | 5 | 3 | [run](https://argusic.com/run/2796610b-6642-4db2-9cd1-a7f46d20fd79) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `No pnpm/Bun/tmux in container; Node 18 below engines (>=20)`
- 3 min: `tmux-ide init crashed (ENOENT templates/default.yml) on the npm dist`
- 20 min: `send/ls/adopt/status launched bare 'tmux' (ENOENT) with no system tmux`
- 2 min: `development-container-app tests fail: /usr/bin/ssh missing in container`
- 4 min: `Desktop Vite build fails loading workspace .ts main (ERR_UNKNOWN_FILE_EXTENSION) under Node 22`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
