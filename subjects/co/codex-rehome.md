# codex-rehome

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CalebYcj/codex-rehome, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/codex-rehome

## Pinned environment

- Project commit: `121ba939bbee068d7d11f410121887bf2df011c3`
- Test commit: `121ba939bbee068d7d11f410121887bf2df011c3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 53.7 to 53.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 55 | 53.7 | 7 | 7 | [run](https://argusic.com/run/12ebafa0-6548-441a-af56-e637881f5d93) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain not installed`
- 8 min: `Missing system dev libraries (glib-2.0, gtk+-3.0, webkit2gtk-4.1, libsoup-3.0, JavaScriptCoreGTK)`
- 3 min: `updater:default capability permission not found on Linux (tauri-plugin-updater excluded on Linux in Cargo.toml and lib.rs)`
- 5 min: `Linker (lld) could not find webkit2gtk, soup, and JavaScriptCore .so files (broken symlinks in sysroot)`
- 3 min: `7 bridge tests failed: restore target paths must be absolute`
- 2 min: `discovery_reports_fixture_without_modifying_it panicked: is_forbidden() matched tmp in /tmp/... path`
- 1 min: `legacy_test: schema_v3_payloads_enter_the_normal_restore_plan failed same path-absolute error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
