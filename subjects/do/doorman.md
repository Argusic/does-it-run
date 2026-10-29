# doorman

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/doorman-dev/doorman, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/doorman

## Pinned environment

- Project commit: `7dcf39f19f7f2c6cdee2a52e740bb01f1b456b9d`
- Test commit: `7dcf39f19f7f2c6cdee2a52e740bb01f1b456b9d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 28.4 to 28.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 25 | 28.4 | 3 | 3 | [run](https://argusic.com/run/0f812b4b-9751-40ac-882e-fc03511f46d5) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Rust 1.88 toolchain missing in container; Node 18 instead of required Node 22`
- 13 min: `Pinned python-parity-reference git ref pointed to HEAD instead of pinned commit 10699820, so scripts/check_parity_reference.py failed`
- 6 min: `Docker unavailable in container; make local-e2e and external-storage suite gate on a Docker daemon and cannot run here`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
