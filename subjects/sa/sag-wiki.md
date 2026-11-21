# SAG-Wiki

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Zleap-AI/SAG-Wiki, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/sag-wiki

## Pinned environment

- Project commit: `816900db41b845318d3235b2b3a4cebd33698990`
- Test commit: `816900db41b845318d3235b2b3a4cebd33698990`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 23.2 to 41.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 21 | 23.2 | 2 | 2 | [run](https://argusic.com/run/e07eeeba-4c71-44f9-b959-b2ec4d7b4ebb) |
| 2 | pass | 80 | 41.27 | 41.7 | 6 | 0 | [run](https://argusic.com/run/d3295387-085a-4090-ae73-8e4a03703f84) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 is too old for jsdom 30 (requires >=22). Installed nvm and Node 22.`
- 6 min: `html-encoding-sniffer CJS require() cannot load ESM-only @exodus/bytes/encoding-lite.js`

Attempt 2:

- 41.27 min: `8 test files fail at import: jsdom ESM module html-encoding-sniffer uses require() of ES Module @exodus/bytes/encoding-lite.js on Node 18.19.1`
- 41.27 min: `web-clipper-windows.test.js: 8/10 tests fail because crypto global is undefined in Node 18 worker threads`
- 41.27 min: `explore-view.test.ts: 1/15 tests fails with hook timeout in graph renderer animation test`
- 41.27 min: `notice.test.ts: 4/4 timer-based tests fail under happy-dom/vitest timing`
- 41.27 min: `docs-site build requires Node.js >=20.9.0, container has v18.19.1`
- 41.27 min: `Tauri desktop build requires Rust toolchain (rustc/cargo not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
