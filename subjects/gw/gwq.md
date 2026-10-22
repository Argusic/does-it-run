# gwq

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/d-kuro/gwq, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/gwq

## Pinned environment

- Project commit: `c4247734968bc3f66addd1e088c19b962c27cfc1`
- Test commit: `c4247734968bc3f66addd1e088c19b962c27cfc1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.9 to 3.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 3.9 | 3 | 3 | [run](https://argusic.com/run/6bf4f706-5b18-4533-9c6d-f334b1fd0122) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go toolchain not installed on system and no root to install packages`
- 1 min: `gwq add failed: no worktree path generated because scratch repo had no git remote (naming.template requires repository URL)`
- `git fetch origin over https prompted for GitHub username with terminal prompts disabled`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
