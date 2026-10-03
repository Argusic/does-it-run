# auto-editor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WyattBlue/auto-editor, licensed Unlicense, written in Nim.

Evidence and recordings: https://argusic.com/subject/auto-editor

## Pinned environment

- Project commit: `eb41d26177deab70262fb41c381f294caa75e060`
- Test commit: `eb41d26177deab70262fb41c381f294caa75e060`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 20 to 39.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23.5 | 34.3 | 6 | 6 | [run](https://argusic.com/run/7dc95e02-e378-4058-a6c2-3436275807c1) |
| 2 | pass | 100 | 20 | 20 | 5 | 5 | [run](https://argusic.com/run/9c192193-842f-4bae-903c-c8b0b1e5a082) |
| 3 | pass | 100 | 36.6 | 39.9 | 6 | 6 | [run](https://argusic.com/run/cd82652e-f5fe-42fa-aabf-cb15e6088b2e) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Missing Nim compiler (required >= 2.2.2)`
- 0.5 min: `Missing nimcrypto dependency`
- 8 min: `FFmpeg 7.0 API (avcodec_get_supported_config, AVCodecConfig enum) not available in system FFmpeg 6.1.1`
- 1 min: `SwsContext type not typedef'd in FFmpeg 6.1.1`
- 1 min: `sws_free_context function (FFmpeg 7) not in FFmpeg 6.1.1`
- 2 min: `Missing -dev packages for FFmpeg and codec libraries`

Attempt 2:

- 5 min: `Nim compiler not found in container`
- 4 min: `nimcrypto dependency not installed`
- 2 min: `zlib tarball download from zlib.net returned HTML (broken CDN)`
- 15 min: `nasm assembler not installed`
- 1 min: `meson and ninja not found (needed by build system)`

Attempt 3:

- 2 min: `FFmpeg dev headers not installed - libavutil/rational.h missing`
- 8 min: `System FFmpeg 6.1 headers missing AVCodecConfig enum needed by FFmpeg 9.x API in Nim code`
- 2 min: `Linker errors: -lmp3lame -lopus -lx264 -ldav1d -lz -lasound not found`
- 4 min: `meson/ninja not installed; makeff task failed on pip install due to externally-managed-environment`
- 12 min: `Encoder not found: h264 at runtime; built FFmpeg without h264 encoder`
- 1 min: `Undefined x264 symbols at link after rebuild`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
