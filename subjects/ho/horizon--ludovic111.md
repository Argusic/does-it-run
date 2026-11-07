# horizon

**Verdict: runs with mocks.** Argusic Score 61 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ludovic111/horizon, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/run/9a497bfd-3cde-4e76-9dc6-65c3dcbd689e

## Pinned environment

- Project commit: `4a675206b1cfff0c4fc401e4058d0c148199c1f3`
- Test commit: `4a675206b1cfff0c4fc401e4058d0c148199c1f3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 16.8 to 32.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 16.8 | 4 | 4 | [run](https://argusic.com/run/9a497bfd-3cde-4e76-9dc6-65c3dcbd689e) |
| 2 | fail | 30 | 4 | 32.9 | 4 | 0 | [run](https://argusic.com/run/79a9e47d-0b64-45d0-a6de-fc6401155839) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `horizon-dualsense cannot build without libudev-dev headers (no root access)`
- 1 min: `horizon-telemetry test this_machine_is_described fails: assertion cores(4) > threads(192) due to container CPU topology reporting 192 processors from /proc/cpuinfo`
- `Launcher test a_replaced_binary_is_replaced_again_at_its_path fails: binary size assertion 509 != 493, likely build-toolchain-dependent self-size check`
- `No Vulkan/GPU available in headless container: client fails to create surface on DISPLAY=:99`

Attempt 2:

- `horizon-client: cannot launch game without prepared Minecraft 26.3 resources (.local/). Requires a real Minecraft installation and JDK 25 for one-time prepare.`
- 1 min: `horizon-telemetry: test system::tests::this_machine_is_described fails in container because /proc/cpuinfo shows 192 CPUs (all threads) while available_parallelism respects cgroup limit of 4, violating cores <= threads assertion. Not fixable`
- 5 min: `horizon-launcher: cannot link due to missing libxcb-dev and libxkbcommon-dev .pc files. Runtime libs (.so) exist but dev headers/pkgconfig files missing. No root to install packages.`
- `horizon-dualsense: cannot compile due to missing alsa-sys (alsa.pc not found). No root to install libasound2-dev.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
