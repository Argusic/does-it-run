# usque-app

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GeorgeXie2333/usque-app, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/usque-app

## Pinned environment

- Project commit: `1d44597ddb6dee7fca6700c0442e0d3856eea31b`
- Test commit: `1d44597ddb6dee7fca6700c0442e0d3856eea31b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 25.5 to 25.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 25.5 | 5 | 5 | [run](https://argusic.com/run/c6696a17-7dd2-4777-962e-23618932547e) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `boring-sys build failed: 'Unable to find libclang' , no libclang on system`
- 1 min: `boring-sys: 'fatal error: stddef.h file not found' , clang built-in headers missing`
- `5 usque-transport tests fail with AddrNotAvailable , IPv6 kernel disabled in container`
- `15 usque-update tests fail , require privileged filesystem operations (uid/perm checks on system paths)`
- `Flutter GUI (apps/usque_gui) not built , Flutter SDK not available, no root to install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
