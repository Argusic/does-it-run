# vector

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vectordotdev/vector, licensed MPL-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/vector

## Pinned environment

- Project commit: `3ce105431bedb23949001e26420c3c614dac2d8f`
- Test commit: `3ce105431bedb23949001e26420c3c614dac2d8f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 70.9 to 77.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 45 | 70.9 | 6 | 6 | [run](https://argusic.com/run/89f7d9b2-89f7-44d1-872a-c16c8cce2b7b) |
| 2 | pass | 100 | 76 | 77.6 | 7 | 7 | [run](https://argusic.com/run/c19a178c-86cc-4edf-96b2-c0daa848244a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain not installed`
- 2 min: `unzip not available for protoc extraction`
- 20 min: `libclang.so not found - required by bindgen crate`
- 10 min: `Full binary linking OOM (SIGKILL)`
- 2 min: `Disk full during build (40GB filesystem)`
- `3 pre-existing test failures in secrets::exec::tests (missing external binary)`

Attempt 2:

- 1 min: `scripts/environment/install-protoc.sh failed: unzip: command not found`
- 6 min: `cargo build --bin vector failed in zstd-sys because libclang.so was missing`
- 2 min: `bindgen then failed with zstd.h:10: fatal error: stddef.h file not found`
- 27 min: `Full default cargo build was killed by the cgroup OOM killer at the 8 GB memory limit`
- 2 min: `Three secrets::exec tests failed with No such file or directory because python was not installed under that name`
- 6 min: `Four config::watcher tests failed with Too many open files when run together; the container permits only one inotify instance`
- 4 min: `make test using nextest failed after cargo test compilation with No space left on device`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
