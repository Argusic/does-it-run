# usagi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/brettchalupa/usagi, licensed Unlicense, written in Rust.

Evidence and recordings: https://argusic.com/subject/usagi

## Pinned environment

- Project commit: `a0a91abe5659b9bb2bb73eee0f899eec723205bc`
- Test commit: `a0a91abe5659b9bb2bb73eee0f899eec723205bc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 37.8 to 37.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 36 | 37.8 | 7 | 7 | [run](https://argusic.com/run/1ba83d86-1ecf-4936-a894-d06eafbe9de8) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `no Rust toolchain in container`
- 10 min: `missing X11/GL dev headers, libclang, zlib dev (no root)`
- 8 min: `CMake cannot see user sysroot (find_path/find_library ignore C_INCLUDE_PATH)`
- 6 min: `bindgen: 'stdarg.h' file not found and libLLVM-18 missing`
- 3 min: `RUSTFLAGS were cleared when building the usagi test binary, so -lGLESv2/-lGLdispatch/-lX11 could not be found by rust-lld`
- 6 min: `Xvfb: rendered game window xwd reads came back all-black (black ground) and XTest fake-key events were initially ignored before focus was set`
- `gif crate (weezl 0.1.12) writes LZW min-code-size 2 with first code 7 instead of clearing (see I: parser, decoder, and ImageMagick all read the stream as 'code 7 >= next 6'), ffmpeg logs 1 'LZW decode failed' per known-buggy frame stream, a`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
