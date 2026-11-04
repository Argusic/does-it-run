# fn-knock-turborepo

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kci-lnk/fn-knock-turborepo, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/fn-knock-turborepo

## Pinned environment

- Project commit: `c9e44e1f1428c4589daed86ae4c54248efb4e67d`
- Test commit: `c9e44e1f1428c4589daed86ae4c54248efb4e67d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 45.6 to 45.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 15 | 45.6 | 12 | 8 | [run](https://argusic.com/run/c879def7-36a7-4aab-90e3-a94fb309ea67) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Container had Node 18.19.1, npm 9.2.0, and no Rust toolchain; README requires Node 22.12+, npm 10.8.2, and Rust 1.96.0.`
- 2 min: `No Go was installed, and the initially installed Go 1.24.6 was below the pinned gateway go.mod requirement of Go 1.26.10.`
- 1 min: `Cloning the sibling gateway into /work failed with permission denied.`
- 1 min: `/usr/bin/time is absent, terminating the first npm ci wrapper before installation started.`
- 1 min: `A harmless cleanup command in the toolchain setup was rejected by the command safety guard.`
- 1 min: `The optional file utility was absent after the Go build.`
- 2 min: `runtime:auth-assets and runtime:auth-single-service could not find the gateway because the shared harness ignored FN_KNOCK_RUNTIME_E2E_GATEWAY_BIN.`
- 3 min: `First runtime:auth-single-service attempt timed out with HTTP 503 from /__fn-knock/readyz during heavy Rust compilation.`
- 31 min: `cargo test failed when rustc was SIGKILLed while linking the lib-test binary; serial --jobs 1 retry was also SIGKILLed at about 6.3 GB RSS.`
- 1 min: `Direct execution of the built Rust integration-test binary failed because CARGO_BIN_EXE_server-admin-rs is only populated by Cargo's test harness.`
- 2 min: `Alternative rust-lld linking failed because the linker could not find libc or GCC runtime libraries.`
- 2 min: `Go suite package pkg/proxy failed the IPv6 dual-stack test because this container cannot bind or reach ::1; an independent Python bind returned OSError 99.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
