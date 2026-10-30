# jazz

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/garden-co/jazz, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/jazz

## Pinned environment

- Project commit: `2a14de32bc7a91e7747a5049adbb84d2d40278ac`
- Test commit: `2a14de32bc7a91e7747a5049adbb84d2d40278ac`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 82.3 to 82.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96.67 | 82 | 82.3 | 6 | 5 | [run](https://argusic.com/run/7927ad8e-15f0-49e7-9eed-0dd81bc17d1b) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Container had Node 18 (repo needs >=22) and no pnpm/corepack; pnpm install could not run`
- 8 min: `No Rust toolchain (rustc/cargo missing)`
- 18 min: `RocksDB bindgen failed: Unable to find libclang (no libclang-dev, no root to install it)`
- 10 min: `cargo test aborted with 'thread has overflowed its stack' on default 2MB test threads`
- 3 min: `Browser (vitest playwright) tests failed: chromium_headless_shell-1208 executable missing`
- 6 min: `auth-simple-chat browser test 2/3 fail: AccountAuthError invalid_identity_token because test JWTs lack an iss claim required by identityFromToken`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
