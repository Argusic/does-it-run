# microduck

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pollen-robotics/microduck, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/microduck

## Pinned environment

- Project commit: `a9ec4b2079ef8ee7904014089c885bb07d57d63c`
- Test commit: `a9ec4b2079ef8ee7904014089c885bb07d57d63c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 37.6 to 37.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 45 | 37.6 | 4 | 4 | [run](https://argusic.com/run/8da552ca-fd02-4f42-9a6a-fb4916f757e2) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Missing rustc toolchain - none installed`
- 20 min: `Missing -dev packages: libudev-dev, libglib2.0-dev, libgstreamer1.0-dev, libgstreamer-plugins-base1.0-dev, libgstreamer-plugins-bad1.0-dev - no root access to apt`
- 5 min: `Linker could not find -ludev (broken symlinks in extracted -dev packages)`
- 3 min: `mediad test failed at runtime: missing libdw.so.1, liborc-0.4.so.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
