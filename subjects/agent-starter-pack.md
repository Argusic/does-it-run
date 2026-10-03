# agent-starter-pack

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GoogleCloudPlatform/agent-starter-pack, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agent-starter-pack

## Pinned environment

- Project commit: `659f047742457bd55e5db0edd088cf678b6f0669`
- Test commit: `659f047742457bd55e5db0edd088cf678b6f0669`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 7.7 to 21.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 3 | 21.6 | 1 | 1 | [run](https://argusic.com/run/a3cdf4c5-35b4-45ac-9418-c70760c845ab) |
| 2 | pass | 100 | 5 | 7.7 | 1 | 1 | [run](https://argusic.com/run/fbf38182-c3e0-4948-bd1d-21f6c5de37dd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `uv not found in PATH in isolated test environment, causing test_smart_merge_preserves_user_dependencies to fail because subprocess could not resolve 'uv' binary`

Attempt 2:

- 2 min: `test_smart_merge_preserves_user_dependencies failed because uv was not in PATH, causing _write_dependencies_to_pyproject to log 'uv not found' and return False`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
