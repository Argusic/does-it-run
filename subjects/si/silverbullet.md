# silverbullet

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/silverbulletmd/silverbullet, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/silverbullet

## Pinned environment

- Project commit: `7cf23a9761e7a1923a5772da76cf5dc002b65727`
- Test commit: `7cf23a9761e7a1923a5772da76cf5dc002b65727`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 18.5 to 30.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 20 | 18.5 | 2 | 0 | [run](https://argusic.com/run/071007b8-1182-4c90-8468-5b5a6d6844c1) |
| 2 | pass | 100 | 23 | 30.1 | 4 | 4 | [run](https://argusic.com/run/25a9a176-bf97-4063-8188-2d4606b4b341) |

## What was observed on a clean machine

Attempt 1:

- `ssh-keygen not found - 11 Rust tests fail requiring openssh-client (git SSH key management)`
- `Chrome/Chromium not found - runtime API disabled (headless Chrome for server-side Lua)`

Attempt 2:

- 7 min: `System Node.js was v18.19.1 but the project requires Node 24+`
- 6 min: `No Rust toolchain installed (rustc/cargo not found)`
- 6 min: `cargo test: 11 revision-sync tests failed because ssh-keygen is missing from the container`
- 4 min: `make setup warned that system libraries required by Playwright/Chromium (libnss3, gstreamer etc.) are absent`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
