# platypush

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/blacklight/platypush, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/platypush

## Pinned environment

- Project commit: `82a233425e1c6d5a763f27dc4865f71a24412690`
- Test commit: `82a233425e1c6d5a763f27dc4865f71a24412690`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.9 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 5.9 | 2 | 2 | [run](https://argusic.com/run/44010a87-20ec-4378-bc21-de62eb2a2b9b) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `redis-server binary not found in PATH causing App to exit during test setup`
- 1 min: `ModuleNotFoundError: No module named 'cryptography' in test_device_auth_response`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
