# intelligent-terminal

**Verdict: could not verify.** Argusic Score 25 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/intelligent-terminal, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/intelligent-terminal

## Pinned environment

- Project commit: `0ed68b9bbf1205d6f0b3e80808b54d52a7b7f886`
- Test commit: `0ed68b9bbf1205d6f0b3e80808b54d52a7b7f886`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 17.5 to 32.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 28 | 17.5 | 4 | 0 | [run](https://argusic.com/run/5b0d2963-7fff-4bd5-b3c0-e77226a20098) |
| 2 | fail | 50 | 38 | 32.2 | 7 | 7 | [run](https://argusic.com/run/1b7ea431-9b5c-41df-8225-913507ab57ca) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Missing Windows PE linker: no link.exe (MSVC target)`
- 5 min: `Missing mingw-w64 cross-compiler (gnullvm target)`
- 3 min: `Missing Visual Studio/MSBuild for C++ Terminal app`
- 2 min: `No Wine to run existing .exe binaries`

Attempt 2:

- 2 min: `Rust toolchain not installed`
- 1 min: `WTA crate uses ms-prod-1.93 toolchain not available in rustup`
- 2 min: `WTA crate uses Windows-only APIs (std::os::windows, tokio::net::windows::named_pipe, win32 sys) , won't compile on Linux natively`
- 5 min: `Missing mingw-w64 cross-compiler for Windows GNU target`
- 1 min: `Missing linker x86_64-w64-mingw32-gcc`
- 2 min: `Missing Windows SDK library -lOneCore_apiset`
- 10 min: `WTA test links to PE binary but cannot execute on Linux (Exec format error)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
