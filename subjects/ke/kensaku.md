# kensaku

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yjid/kensaku, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/kensaku

## Pinned environment

- Project commit: `c2da457a53208fe82ddacda8a37788a879f50cdf`
- Test commit: `c2da457a53208fe82ddacda8a37788a879f50cdf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 40.1 to 40.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 68 | 40.1 | 4 | 4 | [run](https://argusic.com/run/3eba77e0-1a1a-4ced-825d-b7b8f74266ab) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Rust toolchain installed in container`
- 50 min: `Missing system dev libraries: libwebkit2gtk-4.1-dev, libgtk-3-dev, librsvg2-dev, libayatana-appindicator3-dev, patchelf, and ~30 transitive dev packages (no root, can't apt install)`
- 1 min: `Bun not available to run make install`
- `kensaku-daemon binary does not respond to --help (hangs waiting for socket connection)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
