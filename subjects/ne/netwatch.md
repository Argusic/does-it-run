# netwatch

**Verdict: runs.** Argusic Score 98 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/matthart1983/netwatch, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/netwatch

## Pinned environment

- Project commit: `ee7d217438f414fc9eada43190312857834997c7`
- Test commit: `ee7d217438f414fc9eada43190312857834997c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.6 to 23 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 18 | 23 | 5 | 4 | [run](https://argusic.com/run/5d541986-7235-41cf-8afe-2210ee1d336e) |
| 2 | pass | 100 | 12 | 11.6 | 3 | 3 | [run](https://argusic.com/run/d5cad77f-4115-4050-8f61-d88b26a1aa17) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `cargo/rustc not found in container`
- 4 min: `link failed: rust-lld unable to find library -lpcap (no libpcap / no root)`
- 6 min: `runtime/loader error: libpcap.so.0.8 missing; then libibverbs.so.1 and libnl missing (static lib had RDMA symbols)`
- 4 min: `2 conn_view_tests failed asserting selection_bg; container sets NO_COLOR=1 so monochrome::strip resets backgrounds`
- 2 min: `2 collector tests panicked binding ::1: Cannot assign requested address (code 99)`

Attempt 2:

- 6 min: `libpcap-dev not available as system package (no root)`
- 3 min: `system lld not found; rustc uses its bundled lld which couldn't find libpcap when building the binary`
- 3 min: `4 test failures in environment-specific areas (2 IPv6 bind failures since container has no IPv6 loopback; 2 conn_view_tests TUI rendering failures in headless terminal)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
