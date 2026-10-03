# agent-governance-toolkit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/agent-governance-toolkit, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/agent-governance-toolkit

## Pinned environment

- Project commit: `6b644564d112b879e48183bc1655fcf73c86d23e`
- Test commit: `6b644564d112b879e48183bc1655fcf73c86d23e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18 to 18 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17 | 18 | 4 | 4 | [run](https://argusic.com/run/2289a46a-18f2-4303-98b0-22847423f997) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Externally-managed Python environment prevents system-wide pip installs`
- 7 min: `agent-control-specification <0.5.0,>=0.4.0b0 not on PyPI`
- 1 min: `OPA binary not found (required by policy engine)`
- 1 min: `SubprocessSandboxProvider tests fail because 'python' executable not found (only python3 exists)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
