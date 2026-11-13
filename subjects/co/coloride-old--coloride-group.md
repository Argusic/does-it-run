# Coloride-old

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coloride-group/Coloride-old, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/bf384b98-9add-4ed3-bda1-8ff33ecd146a

## Pinned environment

- Project commit: `5c7eab5b265e63f0e142070ff95807631ce23819`
- Test commit: `5c7eab5b265e63f0e142070ff95807631ce23819`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 7.9 to 15.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 15.3 | 0 | 0 | [run](https://argusic.com/run/bf384b98-9add-4ed3-bda1-8ff33ecd146a) |
| 2 | pass | 100 | 12 | 7.9 | 6 | 6 | [run](https://argusic.com/run/e4409abf-4d88-4e18-acd1-a63a075b8b41) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Node.js 18.19.1 installed but project requires Node 22`
- 1 min: `corepack signature verification failed with Node 22.0.0 and corepack 0.36`
- 2 min: `pnpm install --frozen-lockfile did not download Electron binary (lockfile generated on macOS, optional deps skipped)`
- 1 min: `Electron SUID sandbox crash on Linux`
- 1 min: `rolldown native binding @rolldown/binding-linux-x64-gnu not installed (optional dep skipped on frozen install)`
- `test_local_zsh_loads_user_zshenv_and_its_redirected_rc fails - /bin/zsh not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
