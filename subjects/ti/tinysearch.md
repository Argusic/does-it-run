# tinysearch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tinysearch/tinysearch, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/tinysearch

## Pinned environment

- Project commit: `d6c92d5a62cec0a09cb153b4ec55365b20c5aa0b`
- Test commit: `d6c92d5a62cec0a09cb153b4ec55365b20c5aa0b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.1 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 6.4 | 1 | 1 | [run](https://argusic.com/run/80fbf604-126d-416c-a294-cdc9efa58831) |
| 2 | pass | 100 | 9 | 3.1 | 3 | 3 | [run](https://argusic.com/run/cec465a9-967b-4f9a-a387-f43c6b836af3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `WASM target wasm32-unknown-unknown not installed; cargo run --features=bin -- fixtures/index.json failed with 'can't find crate for core' for wasm cross-compilation`

Attempt 2:

- 5 min: `cargo/rustc not found in container`
- 2 min: `integration test test_cli_wasm_mode failed: wasm32-unknown-unknown target not installed`
- `wasm-opt (binaryen) not installed for the optional -o optimization flag`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
