# PoloDB

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PoloDB/PoloDB, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/polodb

## Pinned environment

- Project commit: `55aa7a2fdcb6a1f6402913bf48070a4a9bee3474`
- Test commit: `55aa7a2fdcb6a1f6402913bf48070a4a9bee3474`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 35.6 to 75.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 35.6 | 5 | 5 | [run](https://argusic.com/run/121a95d4-dc55-46bb-b020-975ec491c800) |
| 2 | pass | 100 | 74 | 75.6 | 4 | 4 | [run](https://argusic.com/run/75f20b46-1bad-4d56-b569-f7255df4fdda) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Rust toolchain installed`
- 1 min: `libclang not found for bindgen`
- 1 min: `stdbool.h not found by bindgen (missing clang include paths)`
- 1 min: `Git submodules not initialized`
- `py-binding-polodb fails linking: no libpython3.12 shared library`

Attempt 2:

- 2 min: `No Rust toolchain installed`
- 8 min: `libclang not found for bindgen build dependency`
- 3 min: `libpython3.12.so not found for py-binding-polodb linker`
- 8 min: `polodb server insert handler only read from document sequences (payload type 1), not main payload`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
