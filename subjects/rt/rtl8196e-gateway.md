# rtl8196e-gateway

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jnilo1/rtl8196e-gateway, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/rtl8196e-gateway

## Pinned environment

- Project commit: `832c833d32b03c46f9dbec5d6f98f1fa91391564`
- Test commit: `832c833d32b03c46f9dbec5d6f98f1fa91391564`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.7 to 5.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 2 | 5.7 | 2 | 1 | [run](https://argusic.com/run/c261f027-dbfe-4ad5-8e59-ebb3b1d3f77b) |

## What was observed on a clean machine

Attempt 1:

- `Missing host packages: fakeroot, mtd-utils, squashfs-tools, tftp-hpa (cannot install without root)`
- `Externally-managed Python environment blocked system-wide pip install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
