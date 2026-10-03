# encore

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/encoredev/encore, licensed MPL-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/encore

## Pinned environment

- Project commit: `13dfbf46f2621dc9456458b735cb2a5f0db15e6a`
- Test commit: `13dfbf46f2621dc9456458b735cb2a5f0db15e6a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 45.1 to 45.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 45.1 | 5 | 5 | [run](https://argusic.com/run/2087668e-ea6a-4aec-9fd8-e0b6380a963c) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Missing libclang for Rust bindgen crate; LLVM 18 requires libtinfo.so.5 which is absent`
- 3 min: `Missing protoc for Rust prost-build crate`
- 5 min: `Rust bindgen can't find stddef.h via LLVM 17's clang`
- `Go test pkg/clientgen fails: whitespace (tab vs space) diffs in generated Go client code golden files`
- `Go test v2/compiler/build fails: runtime.exitEncoreG / runtime.startEncoreG relocation targets not defined`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
