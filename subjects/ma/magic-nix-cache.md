# magic-nix-cache

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DeterminateSystems/magic-nix-cache, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/magic-nix-cache

## Pinned environment

- Project commit: `5a7f052c8f0c6511bbef3570eeed4d39242171ef`
- Test commit: `5a7f052c8f0c6511bbef3570eeed4d39242171ef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 19.9 to 37.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 5 | 19.9 | 1 | 1 | [run](https://argusic.com/run/04c60a71-9e24-446a-b566-e52a9eec9b27) |
| 2 | pass with mocks | 92 | 8.5 | 37.3 | 2 | 2 | [run](https://argusic.com/run/f4921dc9-ff37-42e4-a30e-7789f1787c27) |

## What was observed on a clean machine

Attempt 1:

- 30 min: `Cargo build failed: attic crate requires Nix C++ development libraries (nix-expr, nix-store, nix-util, nix-main) which are not available in the container. The project is designed to be built via the Nix package manager (flake.nix) and depen`

Attempt 2:

- 2 min: `gha-cache failed: protoc not found`
- 35 min: `magic-nix-cache failed: attic C++ bridge requires Nix C++ headers and libnixstore.so`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
