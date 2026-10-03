# turso

**Verdict: runs.** Argusic Score 86.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tursodatabase/turso, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/turso

## Pinned environment

- Project commit: `554ae1b4190a34d785371fa175bf431b01ce201d`
- Test commit: `554ae1b4190a34d785371fa175bf431b01ce201d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 33.7 to 72.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 3 | 33.7 | 3 | 0 | [run](https://argusic.com/run/7e7e2eaf-a837-4c96-a506-b361c0fc6155) |
| 2 | pass | 100 | 35 | 72.4 | 4 | 4 | [run](https://argusic.com/run/c2b1bffd-03b2-4ad2-85b9-9545aae2cfb8) |
| 3 | pass | 80 | 13.2 | 52.4 | 3 | 0 | [run](https://argusic.com/run/c958294c-42b0-47e5-9f25-9767d6f6e8ed) |

## What was observed on a clean machine

Attempt 1:

- `tclsh not installed - cannot run TCL compatibility tests`
- `attached_reader_does_not_pin_read_mark_until_checkpoint_gate_is_available flaky panic-in-destructor during full suite`
- `core_tester integration tests timed out at 300s`

Attempt 2:

- 15 min: `libpython3.12.so missing: py-turso (Python binding) crate cannot link`
- 15 min: `libclang missing + protobuf-c compilation errors: pg_query crate (Postgres parser) fails to build`
- 1 min: `memory-benchmark: #[global_allocator] conflict with turso crate`
- `86 MVCC tests failed on rerun (all in experimental mvcc:: namespace)`

Attempt 3:

- `py-turso: libpython3.12-dev not installed; cannot link libpython3.12`
- `postgres crates (pg_query via bindgen): libclang not installed; cannot generate bindings`
- `turso_core --lib test: mvcc::database::tests::attached_reader_does_not_pin_read_mark_until_checkpoint_gate_is_available panics with SIGABRT when run with other tests (destructor ordering issue); passes in isolation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
