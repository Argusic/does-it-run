# loopx

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/loopx-project/loopx, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/loopx

## Pinned environment

- Project commit: `d42adb874d042a039e5846ea19c4e3acba04b655`
- Test commit: `d42adb874d042a039e5846ea19c4e3acba04b655`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 59.1 to 59.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 59.1 | 3 | 3 | [run](https://argusic.com/run/7c1f4362-ec28-42e4-a6c1-2e7d2565840b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18.19.1 was installed but project requires Node.js >=22.22.3 for the TypeScript control plane runtime`
- 5 min: `tests/control_plane/test_reviewed_promotion_cli.py failed to collect: ImportError for _workspace, _cli, _command, _env, REPO_ROOT from refactored module`
- 2 min: `Python externally-managed-environment prevented system-wide pip install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
