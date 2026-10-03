# takumi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kane50613/takumi, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/takumi

## Pinned environment

- Project commit: `3141f1e5f14a0f41deb00ac8cde908423e8abe32`
- Test commit: `3141f1e5f14a0f41deb00ac8cde908423e8abe32`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 4; wall time 30.6 to 43.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 43.9 | 3 | 3 | [run](https://argusic.com/run/bc0bbe52-1566-4e74-81a6-64ef2e86f025) |
| 1 | pass | 100 | 18 | 34.9 | 3 | 3 | [run](https://argusic.com/run/e669c8c8-65f9-4997-8577-2e6e7c7ab14a) |
| 2 | pass | 100 | 17.2 | 30.6 | 1 | 1 | [run](https://argusic.com/run/e07b156e-4ac7-475f-9789-dcf8e94b460c) |
| 3 | pass | 100 | 39 | 42.9 | 3 | 3 | [run](https://argusic.com/run/47768346-17cf-430a-9ba3-f2578c7d3fcb) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Rust fixture tests failed because format_generated_html invoked oxfmt with Node 18 which doesn't support the 'gv' regex flag in oxfmt's dependencies`
- 5 min: `The root 'bun run build' script uses 'bun --filter '*' run build' which is not a valid bun v1.4 workspace filter command`
- 5 min: `Node 18 (v18.19.1) is installed but all modern tooling (tsdown/rolldown, oxfmt, napi CLI) requires Node >= 20.19, causing import errors with 'node:util.styleText' and 'gv' regex flag`

Attempt 1:

- 3 min: `oxfmt binary failed due to Node.js 18 missing regex 'v' flag (used in tests)`
- 10 min: `napi build and tsdown fail with Node.js 18 because @inquirer/core and tsdown use styleText() from node:util (Node >=21.7)`
- 2 min: `Bun unzip dependency missing from container`

Attempt 2:

- `Integration tests in example/ directories failed: cloudflare-workers, tanstack-start, waku-ssr need wrangler/tanstack/waku toolchains not installed`

Attempt 3:

- 2 min: `Node.js v18.19.1 is too old for napi-rs CLI (@inquirer/core uses styleText from node:util)`
- 3 min: `Node.js v18.19.1 too old for tsdown/rolldown (styleText in node:util)`
- 5 min: `oxfmt test validation failed because oxfmt's CLI script uses regex flag /gv (requires Node 20+)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
