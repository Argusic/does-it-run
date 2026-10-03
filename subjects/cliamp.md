# cliamp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bjarneo/cliamp, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/cliamp

## Pinned environment

- Project commit: `d40cb792b606fd5ac37b63dd24a516f79af65a98`
- Test commit: `d40cb792b606fd5ac37b63dd24a516f79af65a98`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 7.5 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 8.2 | 3 | 3 | [run](https://argusic.com/run/707ce1fb-d8fa-4f8d-955c-e0d34be6d750) |
| 2 | pass | 100 | 15 | 10.1 | 3 | 3 | [run](https://argusic.com/run/e15a920d-8df0-4645-a3d2-44e80617392d) |
| 3 | pass | 100 | 12 | 7.5 | 3 | 3 | [run](https://argusic.com/run/664577e7-3dcd-4659-8c8f-70dfc1f3e5d7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not installed`
- 3 min: `Missing -dev headers (alsa, ogg, vorbis, flac, mpg123) for pkg-config`
- 1 min: `Broken symlinks in extracted .so files (libasound.so -> libasound.so.2.0.0 not in rootfs)`

Attempt 2:

- 3 min: `Go binary not found in PATH (no goenv/mise/asdf)`
- 8 min: `CGO link failed: missing -dev packages for ALSA, FLAC, Ogg, Vorbis, mpg123`
- 4 min: `Linker could not find -lasound/-lFLAC/-lmpg123/-logg/-lvorbis/-lvorbisenc after first attempt`

Attempt 3:

- 5 min: `Go 1.26+ required but not installed (no root)`
- 5 min: `Missing -dev packages for CGO (libasound2-dev, libflac-dev, libvorbis-dev, libogg-dev, libmpg123-dev) , no root for apt`
- 2 min: `Linker cannot find libmpg123, libasound: .so symlinks point to .so.* not in extraction tree`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
