# paperclip

**Verdict: runs.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/paperclipai/paperclip, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/paperclip

## Pinned environment

- Project commit: `7bb6cebeae727a16c205bb80b5c2b9e92ea6b5fa`
- Test commit: `7bb6cebeae727a16c205bb80b5c2b9e92ea6b5fa`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 20.8 to 85 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 34 | 37.8 | 2 | 0 | [run](https://argusic.com/run/4a78ddc0-8344-4d6b-8eb9-bb8e475986af) |
| 2 | pass | 100 | 20.1 | 20.8 | 4 | 4 | [run](https://argusic.com/run/a05da906-395f-4e70-adbc-3c7dfbd9727c) |
| 3 | pass | 96 | 8 | 85 | 5 | 4 | [run](https://argusic.com/run/3126611b-6edc-4167-9f9f-a266cd0297ab) |

## What was observed on a clean machine

Attempt 1:

- `adapter-utils vitest config references non-existent packages/shared path`
- `CLI company-import-transfer test has 1 pre-existing failure`

Attempt 2:

- 1 min: `pnpm not installed in container`
- 3 min: `Node.js v18.19.1 installed but repo requires >=24.11.0`
- `Rust/cargo not available in container , paperclip-runner build and typecheck fails`
- `IPv6 disabled on container causes server test EADDRNOTAVAIL errors when binding ::1`

Attempt 3:

- 2 min: `Container has Node.js 18, needs >=24.11.0`
- 1 min: `pnpm not found`
- 1 min: `cargo/rustc not found - needed for @paperclipai/paperclip-runner Rust binary`
- 1 min: `IPv6 disabled at kernel level (net.ipv6.conf.lo.disable_ipv6=1) causes EADDRNOTAVAIL on ::1 connections, breaking ~350 tests`
- `local-service-supervisor.test.ts: 1 test fails - pre-existing flaky test depending on /proc/net/tcp PID resolution`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
