# wreq-js

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sqdshguy/wreq-js, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/wreq-js

## Pinned environment

- Project commit: `3e5c4d4bde7a9ec4280a458fb9577d425095df10`
- Test commit: `3e5c4d4bde7a9ec4280a458fb9577d425095df10`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 28.2 to 28.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 27 | 28.2 | 6 | 6 | [run](https://argusic.com/run/80fbe0de-4e60-447f-bef8-075e6ab75e1f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18 system-installed, need >=20`
- 1 min: `No Rust toolchain`
- 15 min: `Rust build from source fails , btls-sys crate needs libclang for bindgen, and system has no libclang-dev. Downloaded libclang deb but still missing clang resource files for stddef.h`
- 2 min: `Prebuilt binary missing setCookies (plural) , the Rust source exports fn set_cookies but the published binding predates that addition`
- 2 min: `wreq Rust HTTP library drops non-UTF8 header byte sequences , test expects raw latin1 Location header bytes`
- 2 min: `5 session tests requiring native setCookies (sameSite validation, batch error rollback, expired cookie filtering) cannot run with JS polyfill`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
