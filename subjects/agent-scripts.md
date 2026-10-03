# agent-scripts

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/steipete/agent-scripts, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/agent-scripts

## Pinned environment

- Project commit: `d15557c94fa1b92870d6901dbf07615eadf6dd34`
- Test commit: `d15557c94fa1b92870d6901dbf07615eadf6dd34`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 25.7 to 25.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 2.5 | 25.7 | 4 | 3 | [run](https://argusic.com/run/db72e9e3-9662-4f35-abc3-2326bef4dd10) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `pyyaml Python package not available (system Python managed by apt, no user pip allowed)`
- `No Chrome/Chromium binary available - browser-tools start cannot launch a browser`
- `Ruby psych C extension (YAML parser) could not compile due to missing libyaml system library`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
