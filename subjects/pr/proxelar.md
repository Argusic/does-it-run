# proxelar

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/emanuele-em/proxelar, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/proxelar

## Pinned environment

- Project commit: `d0f2e732de54e12fb4d38a1a1ce886b55f110c2e`
- Test commit: `d0f2e732de54e12fb4d38a1a1ce886b55f110c2e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.6 to 21.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 33 | 21.6 | 6 | 6 | [run](https://argusic.com/run/9a19cdb0-9b81-4db0-afc4-bf69c7335ebc) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `cargo/rustc missing from container; rustup installed 1.97.1 per rust-toolchain.toml`
- 7 min: `boring-sys bindgen failed: libclang not found; then stddef.h/bits/libc-header-start.h not found`
- 6 min: `proxyapi http3 feature failed to compile: boring 5.2.0 has no SslMethod::tls_server/tls_client`
- 7 min: `Two proxyapi tests bound [::1] and failed with AddrNotAvailable (E99) because this container has IPv6 disabled`
- 1 min: `cargo test -p proxyapi --lib -- scripting passed -j to the test binary (Unrecognized option 'j')`
- 3 min: `Repeated reverse-mode 502s during final checks were caused by leftover orphaned proxelar processes from backgrounded shells`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
