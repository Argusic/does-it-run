# Markpad

**Verdict: runs.** Argusic Score 57.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sftwrdotdev/Markpad, licensed BSD-3-Clause, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/markpad

## Pinned environment

- Project commit: `3c92d41dcd4999bfcc5af410a919828d8ce45a26`
- Test commit: `3c92d41dcd4999bfcc5af410a919828d8ce45a26`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 6.9 to 21.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 21 | 21.7 | 4 | 4 | [run](https://argusic.com/run/7215aa95-438e-4d31-98a5-00b4abd4d968) |
| 2 | pass | 95 | 32 | 6.9 | 4 | 3 | [run](https://argusic.com/run/76ff5a0a-7f5f-4065-9407-d3242fba8493) |

## What was observed on a clean machine

Attempt 1:

- `Rust backend build fails , missing system libraries: glib-2.0-dev, libcairo2-dev, libpango1.0-dev, libatk1.0-dev, libsoup-3.0-dev, libwebkit2gtk-4.1-dev, libjavascriptcoregtk-4.1-dev, libgdk-pixbuf2.0-dev, etc.`
- `14 node:test failures from monaco-editor CJS/ESM interop: monaco-editor exports named bindings from CommonJS modules that Node 18 cannot resolve with ESM import syntax`
- `52 vitest/spec tests cannot run , jsdom requires Node 20+; @exodus/bytes/html-encoding-sniffer/webidl-conversions are all ESM-only packages`
- `crypto.randomUUID not available in Node 18 , 3 tabTransfer tests fail`

Attempt 2:

- 5 min: `Node.js v18 too old for jsdom/vitest/marked dependencies`
- 10 min: `Rust not installed`
- 2 min: `Frontend build OOM with default heap`
- `Rust/Tauri backend cannot compile - missing glib-2.0, GTK3, WebKit2 dev packages (need root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
