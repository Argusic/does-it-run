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
- Valid runs: 1; wall time 43.3 to 43.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 43.3 | 4 | 4 | [run](https://argusic.com/run/17ef885f-d5ee-4f80-b622-31f7e863426d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 installed but v26.12.0 required`
- 1 min: `pnpm not found`
- 1 min: `npm global install EACCES due to permissions`
- 15 min: `Container inotify max_user_instances=128 too low for parallel test workers; full suite hangs when fork workers exhaust inotify instances`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
