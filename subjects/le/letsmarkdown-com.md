# LetsMarkdown.com

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Cveinnt/LetsMarkdown.com, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/letsmarkdown-com

## Pinned environment

- Project commit: `4710cf460fff144c60dcc4739a1915de63a323e7`
- Test commit: `4710cf460fff144c60dcc4739a1915de63a323e7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.8 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5.8 | 3 | 3 | [run](https://argusic.com/run/06d9fc77-5e12-4562-877f-8474a49663ed) |
| 2 | pass | 100 | 9.5 | 6.2 | 4 | 4 | [run](https://argusic.com/run/c1d031b7-94ac-48f4-b9e8-8540cdcda241) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `rustc/cargo not installed`
- 1.2 min: `wasm-pack not installed`
- 0.1 min: `wasm-bindgen v0.2.80 incompatible with Rust 1.100.0`

Attempt 2:

- 1.5 min: `Rust toolchain (rustc/cargo) not found in container`
- 1.3 min: `wasm-pack not installed`
- 0.5 min: `wasm-bindgen 0.2.80 incompatible with Rust 1.100 - older crate version on Rust newer than v1.76.0 rejected`
- 0.3 min: `npm install failed because letsmarkdown-wasm/pkg/package.json didn't exist`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
