# dumi

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/umijs/dumi, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dumi

## Pinned environment

- Project commit: `8c4150bf66ad6b46eba8dd38d54b4897b1965740`
- Test commit: `8c4150bf66ad6b46eba8dd38d54b4897b1965740`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 15.6 to 29.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 29.5 | 0 | 0 | [run](https://argusic.com/run/eb2b2e91-412e-48a8-990b-288d06d70e82) |
| 2 | pass | 100 | 14 | 15.6 | 4 | 4 | [run](https://argusic.com/run/225c96bd-7df6-4423-a05d-dfc03f3b912e) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pnpm: not found`
- 3 min: `cargo: not found (Rust toolchain missing)`
- 6 min: `swc_plugin_react_demo.wasm missing (2 techStack tests fail)`
- `node bin/dumi.js --help prints 'Node 20 is required when using utoopack'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
