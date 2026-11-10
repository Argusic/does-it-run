# gluesql

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gluesql/gluesql, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/gluesql

## Pinned environment

- Project commit: `ab43b1a85055cbe60b24edbdc3ea59d69451941f`
- Test commit: `ab43b1a85055cbe60b24edbdc3ea59d69451941f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 10.8 to 19.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.1 | 10.8 | 1 | 1 | [run](https://argusic.com/run/af6c2cdb-47d9-4f6d-b15b-f8eeb2a9f6bf) |
| 2 | pass | 100 | 2.1 | 19.1 | 1 | 1 | [run](https://argusic.com/run/530cd7e8-aa6b-4fb8-99d4-97a8db0f0826) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `git-storage test failed: git user identity not configured, causing 'command_ext::tests::test_command_ext' to panic on 'git status' stderr`

Attempt 2:

- 0.5 min: `git-storage test failed because git user identity was not configured`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
