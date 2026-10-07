# voxtype

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/peteonrails/voxtype, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/voxtype

## Pinned environment

- Project commit: `9c35b72b4fa3635028dfe70b444ca0dc9dcfb389`
- Test commit: `9c35b72b4fa3635028dfe70b444ca0dc9dcfb389`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27.4 to 27.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 27.4 | 4 | 4 | [run](https://argusic.com/run/e19772ca-4172-4004-bf2e-799b671fbdbd) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `rustc/cargo not found`
- 5 min: `alsa-sys build fails: pkg-config cannot find alsa.pc`
- 7 min: `bindgen fails: cannot open libclang shared library (libLLVM.so.18.1 missing)`
- 2 min: `linker: unable to find -lasound`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
