# orca-q

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cin12211/orca-q, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/orca-q

## Pinned environment

- Project commit: `dc786eac873716bfd7f7b1cc3aa1c3829ad54b7b`
- Test commit: `dc786eac873716bfd7f7b1cc3aa1c3829ad54b7b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.5 to 37.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 37.8 | 6 | 6 | [run](https://argusic.com/run/8df0a743-52cc-4ef7-b8e1-399847fd8202) |
| 2 | pass | 100 | 6.5 | 14.5 | 4 | 4 | [run](https://argusic.com/run/bd7bccdf-8026-45ac-935f-10a98b7f7169) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Node.js 18 too old; npm ERR! ERESOLVE/@nuxtjs/storybook peer conflict; require() of ESM module failed`
- 8 min: `vitest.config.ts uses ESM import of @nuxt/test-utils/config, fails with ERR_REQUIRE_ESM`
- 8 min: `TypeScript errors: echarts module not found (10 files), Shimmer.vue computed type, RedisKeyValueViewer defineModel overload, @typed-router/__routes not found`
- 2 min: `EMFILE too many open files (stale node_modules_old from previous install)`
- 2 min: `Nuxt build OOM (node --max-old-space-size=8192 runs out of memory in container)`
- 1 min: `postinstall electron-builder install-app-deps fails (no Electron binary/display deps)`

Attempt 2:

- 0.2 min: `npm peer dep conflict @nuxtjs/storybook requires storybook@~9.0.5 vs root ^10.4.1`
- 3 min: `Node.js v18.19.1 lacks node:util.styleText needed by @clack/core`
- 0.2 min: `postinstall electron-builder crashes on require() of ESM module @noble/hashes/blake2.js`
- 1 min: `Missing echarts dependency , build failed resolving echarts/charts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
