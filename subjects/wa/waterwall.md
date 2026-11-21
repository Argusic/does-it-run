# WaterWall

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/radkesvat/WaterWall, licensed MPL-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/waterwall

## Pinned environment

- Project commit: `9e46105301c53cfa1aa3db232a9d429338f6ed79`
- Test commit: `9e46105301c53cfa1aa3db232a9d429338f6ed79`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 76.4 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/06d28783-b593-4dd4-8ebb-dff506e2790a) |
| 2 | pass | 100 | 32 | 76.4 | 4 | 4 | [run](https://argusic.com/run/f587073d-bf7b-452b-85c0-68c364ab372d) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `ninja build system not installed`
- 1 min: `ip (iproute2) not installed, WATERWALL_ENABLE_INTEGRATION_TEST_NETNS requires it`
- 3 min: `C-only warning flags (-Wmissing-prototypes, -Wnested-externs, -Wstrict-prototypes) leaked into C++ compilations via PUBLIC target_compile_options on ww target, causing -Werror failures`
- `9 unit tests fail due to pre-existing issues: 2 need ip command (environment), 4 hit mimalloc assertion failures in failure-injection tests, 2 fail debugAssertZeroBuf in mux tests, 1 fails port bind conflict`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
