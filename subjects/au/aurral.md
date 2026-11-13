# aurral

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lklynet/aurral, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/aurral

## Pinned environment

- Project commit: `1244f0fb5ce49787786d093a956a114043faf861`
- Test commit: `1244f0fb5ce49787786d093a956a114043faf861`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.6 to 43.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 43.3 | 4 | 4 | [run](https://argusic.com/run/17ef885f-d5ee-4f80-b622-31f7e863426d) |
| 2 | pass | 100 | 5 | 5.6 | 4 | 4 | [run](https://argusic.com/run/6245deb2-4244-42fe-b705-d0df5067257e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 installed but v26.12.0 required`
- 1 min: `pnpm not found`
- 1 min: `npm global install EACCES due to permissions`
- 15 min: `Container inotify max_user_instances=128 too low for parallel test workers; full suite hangs when fork workers exhaust inotify instances`

Attempt 2:

- 3 min: `Node.js 18.19.1 is installed but the project requires Node 26.12.x (enforced by pnpm engineStrict)`
- 1 min: `pnpm 12.15.0 is not installed globally and npm lacks permissions for global installs`
- 0.5 min: `AURRAL_API_KEY must be at least 32 characters`
- 0.5 min: `No backend/.env file existed for dev/startup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
