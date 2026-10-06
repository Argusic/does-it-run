# OpenCCU

**Verdict: runs with mocks.** Argusic Score 48.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenCCU/OpenCCU, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/openccu

## Pinned environment

- Project commit: `d2ceebb53fe8eadfca8576414ef83bf174a530c5`
- Test commit: `d2ceebb53fe8eadfca8576414ef83bf174a530c5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 6.4 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 5 | 0 | 10.2 | 4 | 1 | [run](https://argusic.com/run/98aaddbc-786b-41a4-8035-fe32ae991b5e) |
| 2 | pass with mocks | 92 | 5 | 6.4 | 1 | 1 | [run](https://argusic.com/run/87ab993a-acf1-4a83-b449-3cf2ed782dd0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_rgb_led test_corrupt_saved_state_uses_safe_boot_default failed: runtime mkdir created mode 0775, LedController safety check requires mode 0755`
- `test_devicetypes_assets and test_version_headers need BASE_SOURCE path arg from make check-openccu-base`
- `tclsh not installed; security test (rega_script_injection_test.tcl) not run`
- `make build needs wget (not installed; curl available) and root/kernel toolchain for full firmware build`

Attempt 2:

- 2 min: `test_rgb_led.py: test_corrupt_saved_state_uses_safe_boot_default failed with "unsafe runtime directory" due to umask=002 creating group-writable runtime dir`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
