# HomeTiles

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GalusPeres/HomeTiles, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/hometiles

## Pinned environment

- Project commit: `e0acbc94628d5592f859a364b0153dfb86103498`
- Test commit: `e0acbc94628d5592f859a364b0153dfb86103498`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 25.9 to 25.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 78 | 25.9 | 6 | 6 | [run](https://argusic.com/run/6c1a0cc7-c941-480e-a7ba-28eb33d3ee6e) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Stale generated Web assets: generate-web-assets.mjs --check reported src/web/generated/admin_css_gzip.inc stale`
- 15 min: `6 host C++ tests failed to compile: enum/int comparisons in ternaries (GCC 13 -Werror=extra) in swipe_gestures.h, clock_format.h, text_options.h, tile_config.h`
- 8 min: `Host harness test-settings-access-record.mjs failed: -Werror=class-memaccess on memset of non-trivial DeviceConfig`
- 5 min: `Host harness test-tile-update-service.mjs failed: -Werror=sign-compare in unsigned/int asserts`
- 12 min: `HomeTiles.ino is a bare .ino file, so arduino-cli resolves the sketch name from the directory basename (repo.ino), not the file`
- 2 min: `Initial compile failed: missing version.txt in build root (fatal include in firmware_version.h)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
