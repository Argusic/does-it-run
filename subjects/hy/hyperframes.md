# hyperframes

**Verdict: runs.** Argusic Score 98.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/heygen-com/hyperframes, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/hyperframes

## Pinned environment

- Project commit: `61ba800a5db0825afb40f061fb6df5498dfdb37d`
- Test commit: `61ba800a5db0825afb40f061fb6df5498dfdb37d`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 17.8 to 68.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 17.8 | 9 | 9 | [run](https://argusic.com/run/ac0b46a2-a80d-4aa4-9afd-11c08feafc86) |
| 2 | pass | 94.29 | 37 | 37.7 | 7 | 5 | [run](https://argusic.com/run/229ce5cc-c066-4482-9d60-71b0ad72767f) |
| 3 | pass | 100 | 74 | 68.8 | 5 | 5 | [run](https://argusic.com/run/b9d400ff-114a-4b7f-ba1b-78148aa9a1d0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `bun not found in container`
- 2 min: `Node.js v18.19.1 too old (requires >=22)`
- 1 min: `ffmpeg not found`
- 1 min: `unzip not found (needed for bun installer)`
- 2 min: `build fails: @hyperframes/sdk-playground , Vite config cannot resolve .ts imports from @hyperframes/sdk exports`
- `@hyperframes/cli test: 1 pid-related test fails (activeServerOnPort expects container PID but gets 999999)`
- `@hyperframes/engine test: 7 tests fail , audio FX needs Chrome, ffprobe version mismatch with PNG metadata`
- `@hyperframes/core/test: 101 ERR_REQUIRE_ESM errors from html-encoding-sniffer dependency (bun Node.js compat issue)`
- `@hyperframes/lint test: 14 ERR_REQUIRE_ESM errors, no tests defined`

Attempt 2:

- 2 min: `import.meta.dirname undefined in Node.js 18 , rewrite-esm-extensions.ts failed`
- 1 min: `node:path doesn't export fileURLToPath in Node 18`
- 2 min: `scripts/package-subpaths.mjs uses import.meta.dirname`
- 1 min: `packages/player/scripts/verify-runtime-pin.mjs uses import.meta.dirname`
- 1 min: `packages/gcp-cloud-run/check-dockerfile-workspaces.mjs uses import.meta.dirname`
- 2 min: `sdk-playground vite build: Node 18 cannot handle TypeScript imports`
- `jsdom ESM compatibility in @exodus/bytes causes 9 Studio test failures`

Attempt 3:

- 2 min: `Node.js v18 provided, project requires v22+`
- 1 min: `bun not installed`
- 1 min: `SDK package.json exports pointed import to .ts sources, breaking Vite/Node resolution`
- `lsof not available: CLI portUtils test reports the self-reported PID instead of the OS-confirmed PID`
- `Producer shader transition worker pool tests fail: Node worker_threads cannot load .ts worker files under vitest -- all 7 failures have the same root cause`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
