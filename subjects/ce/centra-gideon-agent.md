# centra-gideon-agent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Sidiora-Labs/centra-gideon-agent, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/centra-gideon-agent

## Pinned environment

- Project commit: `ca531ee54708f0b5845fafc6dc620202fd3dc719`
- Test commit: `ca531ee54708f0b5845fafc6dc620202fd3dc719`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 47.4 to 47.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | n/a | 47.4 | 4 | 4 | [run](https://argusic.com/run/18a509e0-b06c-486a-b792-be05073dab57) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `Schema compiler mapped every unknown dataclass field to JSON type string, so valid nested hypermid config (features object, enums) failed validation and was reset to off defaults on every load`
- 6 min: `System Rust and Node 22 missing; container Node was v18 and pip editable install would build the Rust daemon and the console`
- `Optional extras slack_sdk not installed, so native gideonai-slack-desk bundle fails to import (non-fatal warnings; gateway still boots and serves)`
- 8 min: `Hypermid host is disabled on a fresh home because its lifecycle needs a reviewed local enrollment (operator install plan) before it can start a daemon`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
