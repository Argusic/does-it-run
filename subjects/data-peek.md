# data-peek

**Verdict: runs.** Argusic Score 95.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Rohithgilla12/data-peek, licensed NOASSERTION, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/data-peek

## Pinned environment

- Project commit: `2ce83b15a9a0ddd2a36afa304efece03af217982`
- Test commit: `2ce83b15a9a0ddd2a36afa304efece03af217982`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 4; wall time 17.9 to 38.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 2.5 | 38.7 | 2 | 1 | [run](https://argusic.com/run/e5e303d6-f8e7-4406-96e2-068fe21e2032) |
| 1 | pass | 100 | 10 | 29.3 | 4 | 4 | [run](https://argusic.com/run/765b7fb9-19ba-484e-b8cd-45e25cf55f68) |
| 2 | pass | 100 | 1.15 | 36.8 | 6 | 6 | [run](https://argusic.com/run/67bec89f-2f2f-4313-8e4a-b6994f7db34d) |
| 3 | pass with mocks | 92 | 2.2 | 17.9 | 3 | 3 | [run](https://argusic.com/run/4af4fccb-5eb4-40c8-a0e1-3df7da88f374) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Node 18.19.1: vitest 4/vite 7 require ESM imports but Node 18 lacks --experimental-require-module. Patched vitest/dist/config.cjs to be self-contained CJS.`
- `3 test files fail (23 tests, all fake-timer): vi.useFakeTimers() causes afterEach/cleanup hang on Node 18. Not fixable without Node 20+ or framework patch.`

Attempt 1:

- 1 min: `pnpm not installed in container`
- 3 min: `Node 18 incompatible with vitest 4 (requires Node >= 20)`
- 5 min: `@tailwindcss/oxide-linux-x64-gnu native binding missing (engine-strict filtered it due to Node 18 requirement)`
- 3 min: `electron-vite build failed on renderer: crypto.hash not available in Node 18, used by Vite 7 worker bundling`

Attempt 2:

- 3 min: `Node.js 18 lacks global crypto.randomUUID in vitest renderer tests`
- 2 min: `Array.prototype.toSorted is ES2023, not available in Node 18`
- 8 min: `vitest 4 config.cjs requires() ESM-only packages (std-env, vite) - fails on Node 18`
- 12 min: `vitest 4 vi.useRealTimers() hangs in afterEach hook on Node 18 when setInterval created under fake timers`
- 4 min: `electron-vite build fails: @tailwindcss/oxide native binding not installed (missing optional dependency)`
- 2 min: `electron-vite build fails: crypto.hash is not a function (Node 21+ API)`

Attempt 3:

- 0.5 min: `Vitest 4 requires Node 22+ (ESM-only dependency: std-env), but system Node is 18`
- 2 min: `Vite 7 uses crypto.hash (Node 22+) for worker hashing, failing on Node 18`
- 0.5 min: `@tailwindcss/oxide native binding missing for linux-x64-gnu`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
