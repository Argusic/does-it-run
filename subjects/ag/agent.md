# agent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/buildkite/agent, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/agent

## Pinned environment

- Project commit: `b3d4fce8c492c266ee1728e36e95b48cf1c23245`
- Test commit: `b3d4fce8c492c266ee1728e36e95b48cf1c23245`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23 to 23 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 23 | 3 | 3 | [run](https://argusic.com/run/ab4671f4-5376-4518-9723-3f6131fed3f0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.26.5 not installed on PATH`
- 5 min: `TestPolyglotScriptHooksCanBeRun: ruby not found in $PATH`
- 2 min: `TestResolvingGitHostAliasesWithFlagSupport: ssh binary not found and /etc/ssh/ssh_config.d/ not writable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
