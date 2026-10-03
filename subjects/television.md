# television

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alexpasmantier/television, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/television

## Pinned environment

- Project commit: `8d29bfbc3cf143dab305a5cc21f2fdcb400649bf`
- Test commit: `8d29bfbc3cf143dab305a5cc21f2fdcb400649bf`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 19.6 to 42.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/27cdcfe0-5cc7-43cc-9654-2309e84d3dba) |
| 2 | pass | 100 | 40 | 41.4 | 1 | 1 | [run](https://argusic.com/run/2dec894a-0887-419c-9a59-96dcbb4a074b) |
| 3 | pass | 100 | 3 | 19.6 | 3 | 3 | [run](https://argusic.com/run/11784a1f-362d-4642-992f-553bbac33f25) |

## What was observed on a clean machine

Attempt 2:

- 30 min: `No C compiler (gcc/cc) in container. Rust build scripts (proc-macro2, libc, etc.) cannot link without a C linker and system development libraries (crt1.o, libc.so symlinks).`

Attempt 3:

- 1 min: `Rust toolchain channel '1.98' does not exist as a standalone channel`
- 1 min: `Missing 'fd' binary required by default files channel`
- 2 min: `Missing 'bat' binary required for file previews`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
