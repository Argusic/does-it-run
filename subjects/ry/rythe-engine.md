# Rythe-Engine

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Rythe-Interactive/Rythe-Engine, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/rythe-engine

## Pinned environment

- Project commit: `fa406a5c7000fb0440120f927efca6403770096a`
- Test commit: `fa406a5c7000fb0440120f927efca6403770096a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 24 to 90.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 89 | 90.2 | 11 | 8 | [run](https://argusic.com/run/9f283f1e-641b-4007-9941-3ef7a467223b) |
| 2 | fail | 20 | n/a | 24 | 0 | 0 | [run](https://argusic.com/run/49675425-9c8a-4b9c-babc-38b6e4239250) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `file_solution_handle circular include broke rsl PCH compile`
- 4 min: `variadic rsl assert macros failed with no extra args`
- 25 min: `platform_linux.cpp did not build and Linux filesystem/threading APIs were unimplemented`
- 5 min: `test makefiles lacked catch2 include path`
- 4 min: `test_math.cpp needed FMA but CXXFLAGS lacked it`
- 4 min: `LTO link failed: system ld could not load LLVMgold.so`
- 4 min: `test binaries did not link the catch2 implementation library`
- 3 min: `core-editor shared library failed to link via ld (LLVMgold.so missing)`
- 3 min: `application-module failed: application/context/contexthelper.hpp include path missing`
- 3 min: `rythe-reflection-generator failed: libclang not linked`
- `install/launch needed clang+lld tools not present as system packages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
