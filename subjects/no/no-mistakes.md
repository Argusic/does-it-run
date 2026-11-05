# no-mistakes

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kunchenguid/no-mistakes, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/no-mistakes

## Pinned environment

- Project commit: `ac8e342c54b97a99936dddc238198db342b7b966`
- Test commit: `ac8e342c54b97a99936dddc238198db342b7b966`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 28.6 to 41 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 37 | 41 | 3 | 3 | [run](https://argusic.com/run/036cc804-e6cf-4458-ab76-bbbe6a115bf1) |
| 2 | fail | 80 | 33 | 28.6 | 3 | 3 | [run](https://argusic.com/run/2cbdf973-f8c0-4a6e-a0ca-ad5bcb94edde) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.27.1 was not present in the container environment (no go binary anywhere).`
- `'make build' failed: 'neither GOMODCACHE nor GOPATH is set' because no GOPATH was configured after installing Go.`
- 5 min: `9 tests in 'internal/eval' failed: 'resolveBranchBaseSHA' tried to 'git fetch --no-tags +refs/heads/main:refs/remotes/origin/main' with an empty remote URL, because the eval replay sandbox is an isolated local bare repo with no upstream re`

Attempt 2:

- 3 min: `No Go toolchain installed in container (module requires go 1.25.0)`
- 15 min: `eval replay tests fail: 'git fetch --no-tags +refs/heads/main:refs/remotes/origin/main: fatal: no path specified' - the restoreCase function in internal/eval/replay.go created a worktree with no origin remote`
- 15 min: `eval replay tests still fail: 'git fetch --no-tags origin +refs/heads/main:refs/remotes/origin/main: fatal: couldn't find remote ref refs/heads/main' - the gate had refs/remotes/origin/main but not refs/heads/main`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
