# kapitsa

**Verdict: could not verify.** Argusic Score 10 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nace-ai/kapitsa, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/kapitsa

## Pinned environment

- Project commit: `e21f08b45fde070cb554bb73897e67b547b5c279`
- Test commit: `e21f08b45fde070cb554bb73897e67b547b5c279`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 0.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 0 | 0.9 | 1 | 1 | [run](https://argusic.com/run/52b82829-c777-4ec3-911d-3dbefc74d1aa) |
| 2 | fail | 0 | 12 | 2.9 | 4 | 0 | [run](https://argusic.com/run/f924ac88-fe6c-4bdc-bc38-dd2969cd94f0) |

## What was observed on a clean machine

Attempt 1:

- `Kapitsa requires Apple Silicon (arm64) and macOS 14+ with Xcode Command Line Tools. The environment is x86_64 Linux, which has no Objective-C++ compiler (cc1objplus), no Metal GPU framework, and no Objective-C runtime. CMake configure fails`

Attempt 2:

- 2 min: `Project requires macOS 14+ with Apple Silicon (arm64) , container is x86_64 Linux (Ubuntu 24.04)`
- 5 min: `Objective-C++ compiler (cc1objplus) not available; gobjc++-13 cannot be installed without root`
- 4 min: `CMakeLists.txt hard-codes CMAKE_OSX_ARCHITECTURES arm64 and requires OBJCXX language, Metal, and Apple Neural Engine frameworks`
- 1 min: `No root access to install missing system packages (dpkg lock)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
