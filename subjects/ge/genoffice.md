# genoffice

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/genspark-ai/genoffice, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/genoffice

## Pinned environment

- Project commit: `69b4ce0560a76b64afb617b1495a5ecf79461a93`
- Test commit: `69b4ce0560a76b64afb617b1495a5ecf79461a93`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 17 to 59.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 39.7 | 4 | 4 | [run](https://argusic.com/run/050c40a7-f7a5-4f39-b7bb-cded9c693935) |
| 2 | pass | 100 | 15 | 17 | 3 | 3 | [run](https://argusic.com/run/55d8adbb-6378-46fc-8cd3-1c0c8604d2b4) |
| 3 | pass | 100 | 1.5 | 59.5 | 5 | 5 | [run](https://argusic.com/run/f3676553-9571-4fe0-a4bd-36c7ba873e0b) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Built-in Node.js v18.19.1 too old (needs >=22.12.0)`
- 3 min: `electron postinstall script failed: @electron/get is ESM-only (requires Node >=22)`
- 2 min: `Rust/Cargo not pre-installed for sheets native sidecar`
- 1 min: `Electron SUID sandbox helper abort in container`

Attempt 2:

- 1 min: `Node.js v18.19.1 pre-installed but .nvmrc requires v22; npm complained about unsupported engine for some packages`
- 1 min: `No Rust toolchain (cargo/rustc) on PATH , sheets xlsx sidecar requires it`
- 0.5 min: `Electron SUID sandbox helper not configured (container environment)`

Attempt 3:

- 0.5 min: `Node v18 was installed; repo requires >=22.12`
- 1 min: `Cargo/Rust toolchain not found (needed by sheets xlsx sidecar)`
- 0.5 min: `unzip command not found (used by e2e tests to verify xlsx content)`
- 0.5 min: `zip command not found (used by e2e tests to build .xlsx and .pptx fixtures)`
- 5 min: `5 docs visual regression tests fail: 2305-7617 pixel diffs on committed baselines`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
