# headroom

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/headroomlabs-ai/headroom, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/headroom

## Pinned environment

- Project commit: `5d025f7a03870a402918e6425ca9fcd40400edb2`
- Test commit: `5d025f7a03870a402918e6425ca9fcd40400edb2`
- Worker image digest: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 31.8 to 31.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 31 | 31.8 | 4 | 4 | [run](https://argusic.com/run/223633da-b721-4c17-bad1-e2bb4cdd921a) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `No C compiler (gcc/cc) or binutils in container. Also no pip/venv for Python.`
- 3 min: `C++ compiler needed by esaxx-rs crate (needs cc1plus)`
- 5 min: `GCC fixed include headers (stdint.h) use #include_next which needs system headers in correct search order`
- 3 min: `libc.so linker script has hardcoded absolute paths (/usr/lib/x86_64-linux-gnu/libc_nonshared.a)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
