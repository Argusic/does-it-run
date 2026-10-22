# Connexio

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yandanp/Connexio, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/connexio

## Pinned environment

- Project commit: `67684fcd2ba9cf0213bf152d951fafd5bbd427ac`
- Test commit: `67684fcd2ba9cf0213bf152d951fafd5bbd427ac`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.7 to 23.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 23.7 | 7 | 7 | [run](https://argusic.com/run/06fb615e-6505-4c07-b104-d49788fb4f36) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Rust toolchain in container; rustup minimal lacked rustfmt/clippy`
- 3 min: `npm test failed on system Node 18 (vitest 4: ERR_REQUIRE_ESM, requires Node >=20)`
- 2 min: `oxlint: Cannot find native binding (npm 9 skipped optional @oxlint/binding-linux-x64-gnu under Node 18)`
- 8 min: `No root and system lacks libgtk-3-dev/webkit2gtk-4.1-dev headers; cargo could not find GTK/WebKit pkg-config`
- 5 min: `App crash: spawn WebKitNetworkProcess (No such file or directory) because webkit child binaries live in /usr/lib/x86_64-linux-gnu not visible via LD_LIBRARY_PATH`
- 4 min: `WebKitWebProcess abort: Could not create default EGL display (EGL_BAD_PARAMETER) , sysroot libEGL_mesa missing libgallium`
- 1 min: `WebKit injected bundle not found at /usr/lib system path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
