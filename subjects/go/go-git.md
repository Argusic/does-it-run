# go-git

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/go-git/go-git, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/go-git

## Pinned environment

- Project commit: `e9e5820fe0d23893256d04a0e9f8e9a92db1bc18`
- Test commit: `e9e5820fe0d23893256d04a0e9f8e9a92db1bc18`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27.6 to 27.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 31 | 27.6 | 6 | 6 | [run](https://argusic.com/run/b450fb48-0822-409b-b2fb-f4ff9b59df54) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go binary not installed on system`
- 1 min: `TestPullAdd fails: git commit requires user.email/user.name config`
- 2 min: `boundOS worktree test: container umask 0002 causes 0o664/0o775 instead of 0o644/0o755`
- 1 min: `SSH transport tests fail: no known_hosts file`
- 1 min: `HTTP E2E test fails: missing global git identity`
- `gitignore conformance oracle mismatches git 2.43.0 (pre-existing)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
