# agent-plugins

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/awslabs/agent-plugins, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agent-plugins

## Pinned environment

- Project commit: `097fe8ad56d8a1d5e2c81d7880adf145553cf244`
- Test commit: `097fe8ad56d8a1d5e2c81d7880adf145553cf244`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 7.2 | 5 | 5 | [run](https://argusic.com/run/15faf863-4be0-43aa-ba43-d67c9f1cc540) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `mise was not pre-installed; installed via curl`
- `pip3 blocked by externally-managed-environment policy`
- `pre-commit pipx install hung during initial mise install`
- `semgrep scan killed by SIGTERM during full build (timeout)`
- `checkov timeout scanning the repo`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
