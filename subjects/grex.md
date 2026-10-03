# grex

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pemistahl/grex, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/grex

## Pinned environment

- Project commit: `99cc347707375e00514f938b76d885a201dfc110`
- Test commit: `99cc347707375e00514f938b76d885a201dfc110`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 3.9 to 24.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 24.8 | 2 | 2 | [run](https://argusic.com/run/bd680047-cf68-48d0-949b-38e959a5a4fa) |
| 2 | pass | 100 | 12 | 7.7 | 0 | 0 | [run](https://argusic.com/run/56794dfb-e7d5-4634-a38b-cae27861992f) |
| 3 | pass | 100 | 3 | 3.9 | 2 | 2 | [run](https://argusic.com/run/848c723c-1f2c-44fa-8437-004be3b4112a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Rust toolchain installed`
- 16 min: `linker 'cc' not found , no C compiler in container`

Attempt 3:

- 1 min: `No Rust toolchain present: 'cargo: not found'`
- 1 min: `maturin build failed: 'Cargo metadata failed. Do you have cargo in your PATH?'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
