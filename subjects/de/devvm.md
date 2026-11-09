# devvm

**Verdict: runs with mocks.** Argusic Score 72 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/devvmhq/devvm, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/devvm

## Pinned environment

- Project commit: `eaa170696605e1b02844d1de7bf785869877a8f0`
- Test commit: `eaa170696605e1b02844d1de7bf785869877a8f0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 35.1 to 35.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 3 | 35.1 | 5 | 0 | [run](https://argusic.com/run/50d856e8-c6bb-4c45-b6ac-856319bfee8d) |

## What was observed on a clean machine

Attempt 1:

- `desktop script test fails: nc (netcat) not installed (no apt install without root)`
- `release script test fails: ssh-keygen not installed (needs openssh-client, no root)`
- `4 internal/vm move/adopt tests fail: require interactive terminal (non-TTY environment)`
- `3 opencode tests skipped: sqlite3 binary not installed (no root)`
- `Lima, QEMU, KVM not available (no root, no nested virt)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
