# WinShun

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LingCore/WinShun, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/winshun

## Pinned environment

- Project commit: `911f6876a0f6597b3725bc353a392425aeb0cfb5`
- Test commit: `911f6876a0f6597b3725bc353a392425aeb0cfb5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 35 to 36.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 45 | 35 | 2 | 2 | [run](https://argusic.com/run/8288df4c-b8bf-44dd-81f3-f5274db02763) |
| 2 | fail | 20 | 15 | 36.2 | 2 | 2 | [run](https://argusic.com/run/42b6fb64-cf37-4fdc-b08b-10bc1872c729) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `Top-level CMake hard-fails on Linux: 'WinShun targets Windows only' (Ubuntu 24.04 container, no root, no MSVC/Windows SDK)`
- 15 min: `Official WinShun 0.11.0 portable exited code 53 under wine (missing ICU DLLs followed by unimplemented mscms WcsCreateIccProfile/OpenColorProfileW)`

Attempt 2:

- `Project requires Windows (Win32 APIs: NTFS, BCrypt, COM, shell32, kernel32). Cannot build or run on Linux.`
- 5 min: `Qt 6.8 API ambiguity: QString::arg(int) vs arg(double) with GCC/Clang in ColorText.cpp:80`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
