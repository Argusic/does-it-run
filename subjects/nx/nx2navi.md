# NX2navi

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tangerineturtle1/NX2navi, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/nx2navi

## Pinned environment

- Project commit: `5256959200d2de80123c7f08efa08c77d8b3d696`
- Test commit: `5256959200d2de80123c7f08efa08c77d8b3d696`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 11.9 to 12.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 11 | 11.9 | 0 | 0 | [run](https://argusic.com/run/655c0810-3923-417d-b8d5-d3da4a1b2203) |
| 2 | fail | 50 | 14 | 12.5 | 6 | 6 | [run](https://argusic.com/run/c309a6c6-d321-4d4b-ae3a-18a6f9176152) |

## What was observed on a clean machine

Attempt 2:

- 6 min: `No clang compiler on Ubuntu 24.04 container`
- 1 min: `SDL3 development headers missing (no root to apt install)`
- `Vulkan SDK headers missing`
- `zstd development headers missing`
- `tkinter not available in container`
- `Cannot build game binary in Linux container (targets Windows x86-64 via MSYS2)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
