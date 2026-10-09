# wcap

**Verdict: could not verify.** Argusic Score 0 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mmozeiko/wcap, licensed Unlicense, written in C.

Evidence and recordings: https://argusic.com/subject/wcap

## Pinned environment

- Project commit: `aa25ccb806d7a6e1c0bfdcca863aabcd8e9badfa`
- Test commit: `aa25ccb806d7a6e1c0bfdcca863aabcd8e9badfa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 18 to 19.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 15 | 18 | 3 | 0 | [run](https://argusic.com/run/921f0404-4a46-4b51-91f3-ca4d6c3071a4) |
| 2 | fail | 0 | 15 | 19.3 | 2 | 0 | [run](https://argusic.com/run/ab2940d0-6613-463a-9438-90ed4b2e6aac) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `wcap.c source has 74 compilation errors when cross-compiled with mingw-w64 - missing Windows Graphics Capture API types (contract version 0x130000 required, mingw headers only support 0x60000), including CIDirect3D11CaptureFramePoolStatics,`
- 5 min: `Pre-built wcap-x64.exe (67072 bytes) fails under Wine 9.0 - CoreMessaging.dll not found and is a native Windows 10+ system DLL that Wine does not implement`
- 2 min: `Build system requires Visual Studio (cl.exe), HLSL shader compiler (fxc.exe), and resource compiler (rc.exe) - all Windows-native tools not available on Linux`

Attempt 2:

- 10 min: `wcap.c: 654+ compilation errors when cross-compiling with mingw - missing WinRT/WGC types, DWM_WINDOW_CORNER_PREFERENCE, CoreMessaging.h, and other Windows 10+ API types not available in mingw-w64`
- 5 min: `Prebuilt wcap-x64.exe cannot run under Wine 9.0 - missing unimplemented functions in user32.dll (CreateDialogParamW) and kernel32.dll`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
