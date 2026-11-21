# pyatv

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/postlund/pyatv, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/pyatv

## Pinned environment

- Project commit: `b277a4c8222ecdcbaab8a24e3e713ca44765adb4`
- Test commit: `b277a4c8222ecdcbaab8a24e3e713ca44765adb4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 3.8 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.3 | 3.8 | 0 | 0 | [run](https://argusic.com/run/4ee1225c-cefd-416a-bbd7-590405801ae5) |
| 2 | pass with mocks | 92 | 0.5 | 7.7 | 3 | 3 | [run](https://argusic.com/run/2d37d45b-bfde-4bae-8ddd-0277c80ac097) |

## What was observed on a clean machine

Attempt 2:

- 0.2 min: `PEP 668 externally-managed-environment blocks system pip install`
- 5 min: `test_scan_with_zeroconf_complete_and_device_info_specific_host_matching fails IndexError`
- 1 min: `test_pairing_failed fails TypeError: SRPClientSession.__init__() takes 2 positional arguments but 3 were given`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
