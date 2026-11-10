# sidex

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Sidenai/sidex, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/sidex

## Pinned environment

- Project commit: `ad978652682270a593e7029269beff5411477a70`
- Test commit: `ad978652682270a593e7029269beff5411477a70`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 33.9 to 45.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 45 | 33.9 | 5 | 5 | [run](https://argusic.com/run/6497df2c-12e7-4760-8d52-52301228d9fa) |
| 2 | pass | 100 | 68 | 45.9 | 5 | 5 | [run](https://argusic.com/run/ff2fabed-ff3c-42ab-afca-710509b7f976) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Rust 1.99 API drift: tree_sitter_parser.rs &rust_language() missing &`
- 5 min: `Rust 1.99 API drift: document_color.rs &lsp_info missing &`
- 10 min: `Rust 1.99 API drift: ssh.rs russh_keys PublicKey::from_bytes removed`
- 2 min: `Rust 1.99 API drift: ssh.rs test clone_public_key().ok()! needs unwrap`
- 20 min: `WebKit subprocess binaries at /tmp/sysroot/ not found at hardcoded /usr/lib path`

Attempt 2:

- 5 min: `Rust toolchain not installed`
- 35 min: `No webkit2gtk-4.1-dev, glib-2.0-dev, gtk-3-dev and other system C library development packages`
- 5 min: `Broken .so symlinks in extracted -dev packages (pointed to .so.0 files not in the local prefix)`
- 15 min: `WebKit subprocess helpers (WebKitNetworkProcess, WebKitWebProcess, injected bundle) at hardcoded /usr/lib path not writable by non-root user`
- 8 min: `Runtime libraries for WebKit missing (GStreamer, libxslt, libenchant, etc)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
