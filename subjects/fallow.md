# fallow

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fallow-rs/fallow, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/fallow

## Pinned environment

- Project commit: `86482cc66fe9a331d8477584be5bcba3f99e8923`
- Test commit: `86482cc66fe9a331d8477584be5bcba3f99e8923`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 23.5 to 58.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 38 | 4 | 4 | [run](https://argusic.com/run/4f423d8b-8428-4958-a109-e6625e08b9b7) |
| 2 | pass | 100 | 12 | 23.5 | 2 | 2 | [run](https://argusic.com/run/354085fa-35d9-4d1f-a61f-75468a43e9f5) |
| 3 | pass | 100 | 57 | 58.3 | 3 | 3 | [run](https://argusic.com/run/d888f94e-846a-4635-8869-529067547f17) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not installed`
- 1 min: `Node 18 too old for project scripts (needs Array.prototype.toSorted)`
- 1 min: `pnpm not available for editors/vscode install`
- 3 min: `token_cache_misses_when_only_the_ctime_moved fails on Docker overlayfs where ctime never changes on writes`

Attempt 2:

- 19 min: `Rust toolchain (rustc, cargo) not installed`
- 5 min: `Node.js v18.19.1 too old for type-aware-sidecar (needs >=20); two audit tests failed on toSorted()`

Attempt 3:

- 3 min: `Node.js 18 lacks Array.toSorted() causing fallow-type-aware sidecar failures in 2 tests`
- 1 min: `No Rust toolchain installed`
- 2 min: `cargo test --release p fallow-cli killed by SIGKILL from LTO+release memory`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
