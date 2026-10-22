# ttt

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eugenioenko/ttt, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/ttt

## Pinned environment

- Project commit: `63f10d525283b628246b766cc5973026f2fd9a9a`
- Test commit: `63f10d525283b628246b766cc5973026f2fd9a9a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.8 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 6.8 | 5 | 5 | [run](https://argusic.com/run/c56e2d9f-a84b-4413-9362-c99470b4391d) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go compiler not found on system`
- 0.5 min: `Go trimmed binary requires GOROOT env var`
- 0.5 min: `npm install -g pnpm fails with EACCES (no root)`
- 2 min: `vitest 4.x requires Node >= 20.19.0, only Node 18 present`
- 1 min: `@rolldown/binding-linux-x64-gnu missing from stale pnpm-lock.yaml`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
