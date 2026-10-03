# vibe-kanban

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BloopAI/vibe-kanban, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/vibe-kanban

## Pinned environment

- Project commit: `d5cbb5380fa0b32e98ef9b8d987f63decce4be3a`
- Test commit: `d5cbb5380fa0b32e98ef9b8d987f63decce4be3a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 82.3 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/da7fcaec-26b8-4d29-a9a4-2173329d8b72) |
| 2 | pass with mocks | 92 | 48 | 82.3 | 7 | 7 | [run](https://argusic.com/run/7284b795-1564-4973-a2c9-82ee1babda4d) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Rust toolchain not found (no rustup, cargo, or rustc)`
- 1 min: `pnpm not installed, npm install -g failed due to EACCES on /usr/local/lib`
- 1 min: `.npmrc had engine-strict=true blocking install on Node 18 (requires >=20)`
- 20 min: `libsqlite3-sys build failed: requires libclang for bindgen (no clang-dev installed)`
- 15 min: `LLVM 18.1.8 downloaded first but needed libtinfo.so.5 (NCURSES_TINFO_5.0.19991023 version mismatch)`
- `glib-sys build failure from tauri-app crate (needs GTK/Webkit dev packages)`
- 5 min: `Disk space exhaustion (40GB overlay): cargo test/test binaries and LLVM filled disk`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
