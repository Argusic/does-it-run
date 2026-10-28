# pstop

**Verdict: could not verify.** Argusic Score 31.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/psmux/pstop, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/pstop

## Pinned environment

- Project commit: `8f6a1bc684b140bfa5cd6cb56423e61f5d04d642`
- Test commit: `8f6a1bc684b140bfa5cd6cb56423e61f5d04d642`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 11.9 to 41.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 13.33 | 12 | 11.9 | 3 | 2 | [run](https://argusic.com/run/b2ceea74-d6fa-490e-8828-19cc0fe4bf2a) |
| 2 | fail | 50 | 37 | 41.4 | 3 | 3 | [run](https://argusic.com/run/d5943fa9-839e-46fd-a4e5-4096fffdd55f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Rust toolchain present in container (cargo/rustc missing)`
- 30 min: `cargo build failed: windows-future 0.3.2 (via windows 0.62.2) references cfg(windows)-only windows_core::imp::IMarshal/marshaler and windows_threading::submit on non-Windows`
- 10 min: `pstop source itself is Windows-only: 52 errors in src/system/winapi.rs, src/input.rs, src/system/wsl.rs, src/main.rs calling Win32 APIs (windows::Win32 modules, ntapi::ntexapi, RegQueryValueExW, Command::creation_flags); binary cannot link`

Attempt 2:

- 2 min: `Rust toolchain not installed on system`
- 25 min: `Windows-only crate requires Windows target with MSVC linker unavailable (no link.exe)`
- 8 min: `Cannot run Windows executable without Wine; wine requires missing DLL (zlib1.dll) and full prefix setup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
