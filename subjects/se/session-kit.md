# session-kit

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dob323/session-kit, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/session-kit

## Pinned environment

- Project commit: `3978d9845d6c5a2c2c64c1228c0d9d24c1ea4aff`
- Test commit: `3978d9845d6c5a2c2c64c1228c0d9d24c1ea4aff`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 55.2 to 55.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 55.2 | 2 | 2 | [run](https://argusic.com/run/26b5f94f-ee67-4db1-9390-a1d712a5cc5a) |

## What was observed on a clean machine

Attempt 1:

- 11 min: `shpool not on PATH; preflight failed`
- 1 min: `systemd user manager unavailable (container without systemd init)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
