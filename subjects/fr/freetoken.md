# FreeToken

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FlashML-org/FreeToken, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/freetoken

## Pinned environment

- Project commit: `0d652e73a452d014ac5441a15baa75348e9fcb0a`
- Test commit: `0d652e73a452d014ac5441a15baa75348e9fcb0a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28.2 to 28.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 32 | 28.2 | 4 | 4 | [run](https://argusic.com/run/4986ea59-1202-4793-b57c-9c422df5b627) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `CUDA_HOME and CUDA toolkit not found; setup.py hard-requires it for C++ extensions (pinned_tensor, cpu_moe)`
- 5 min: `PyPI wheel (0.1.3) is missing ROCm arch functions (is_rocm, get_rocm_gfx_arch, _rocm_link_flags) that the repo source has and tests expect`
- 2 min: `ninja binary not on PATH; tvm_ffi subprocess calls fail with FileNotFoundError when JIT-compiling radix C++ kernel`
- 2 min: `python3-dev headers missing; cannot compile row_store C++ extension from repo source`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
