# rustwright

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Skyvern-AI/rustwright, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/rustwright

## Pinned environment

- Project commit: `fca14389e99726bca3210190b905e32663395b5c`
- Test commit: `fca14389e99726bca3210190b905e32663395b5c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 68 to 68 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 68 | 6 | 6 | [run](https://argusic.com/run/2eb4c106-bd8f-4557-8352-9ccbde01614d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Rust toolchain in container (cargo/rustc missing)`
- 8 min: `Linker error 'unable to find library -lpython3.12' (libpython3.12.so absent; no root/apt)`
- 1 min: `Chromium failed to start: posix_spawn chrome_crashpad_handler: Permission denied (13); installer delivered browser helpers without exec bits`
- 6 min: `Node build failed on Node v18.19.1: '@inquirer/core' requires node:util.styleText (Node >=20.13)`
- 45 min: `30 tests in tests/test_rustwright_sync_api.py fail against real Chromium: connect_over_cdp remote-cookie sync (empty cookie set), page.requests() window (20 kept, expected 100), HAR route_fulfill FileNotFoundError leak, navigation-mid-wait`
- 10 min: `Full test_rustwright_sync_api.py run (1639 tests) hangs ~45% in batch mode (flaky Chromium race tests)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
