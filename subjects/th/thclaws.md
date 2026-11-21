# thClaws

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/thClaws/thClaws, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/thclaws

## Pinned environment

- Project commit: `e614db6636b41bda0cffe59ba782a13b9a000b1b`
- Test commit: `e614db6636b41bda0cffe59ba782a13b9a000b1b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 15.5 to 20.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 13 | 15.5 | 3 | 3 | [run](https://argusic.com/run/df864522-f676-478c-bcae-e8a86c6f5744) |
| 2 | pass | 100 | 18 | 20.5 | 5 | 5 | [run](https://argusic.com/run/fd5598bc-a800-4737-918f-927eefbaa00b) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `libdbus-1-dev package not installed (no dbus-1.pc or .so symlink for linker)`
- 1 min: `Node.js 18 is too old for frontend build (Vite 8 needs 20.19+)`
- 4 min: `GUI feature build fails: 30+ GTK/WebKit system -dev packages missing (cairo-sys-rs, glib-sys, atk-sys, wayland-sys, javascriptcore-rs-sys, soup3-sys, etc.)`

Attempt 2:

- 3 min: `Missing libdbus-1-dev headers (needed by keyring crate's secret-service feature)`
- 1 min: `Vite 8 requires Node.js 20+ but system has Node 18`
- 1 min: `rolldown native binding missing after pnpm install (optional dep @rolldown/binding-linux-x64-gnu)`
- 5 min: `GUI/--serve feature not available: missing webkit2gtk-4.1 runtime and dev headers system-wide`
- `7 test failures in providers::thclaws_gateway::tests (PoisonError from shared mutex)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
