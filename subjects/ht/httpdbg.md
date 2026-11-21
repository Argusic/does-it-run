# httpdbg

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cle-b/httpdbg, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/httpdbg

## Pinned environment

- Project commit: `121845b41c19ddaf30b51be0797bc2ff4847d8b3`
- Test commit: `121845b41c19ddaf30b51be0797bc2ff4847d8b3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.9 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 7.2 | 2 | 2 | [run](https://argusic.com/run/f459c6ad-f03f-4722-854e-b49d4d9f230c) |
| 2 | pass | 100 | 1.5 | 2.9 | 1 | 1 | [run](https://argusic.com/run/83e82157-2d48-4629-9722-112447ddc832) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Pytest run failed with 'Address already in use' on port 4909`
- 4 min: `Background local mock HTTP server died between exec sessions, causing a ConnectionRefused in the traced client`

Attempt 2:

- 0.5 min: `pip install failed: externally-managed-environment due to Debian PEP 668 policy`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
