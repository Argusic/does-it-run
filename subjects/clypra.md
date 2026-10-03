# Clypra

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AIEraDev/Clypra, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/clypra

## Pinned environment

- Project commit: `4010bd06d736e55e05346804119dfeaf6c9a450d`
- Test commit: `4010bd06d736e55e05346804119dfeaf6c9a450d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 42 to 63.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/67c5880e-eb0b-4a79-aa00-d3499a7d3355) |
| 1 | pass | 100 | 62 | 63.3 | 7 | 7 | [run](https://argusic.com/run/fad1baec-86e8-45b5-b219-acc3ad5d2adf) |
| 2 | timeout | none | 9 | 44.5 | 6 | 6 | [run](https://argusic.com/run/731d1611-cc5c-4e53-b494-3936d6198ebb) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Node.js v18 is too old for project dependencies (needs >=20)`
- 2 min: `tailwindcss-oxide native binary missing (x86_64-linux-gnu not in default targets)`
- 3 min: `jsdom 29 requires ESM import that fails with Node 18's fork pool`
- 10 min: `vitest runs via pnpm script hung due to old node_modules dirs being scanned`
- 3 min: `clypra-native-core Rust tests missing layer_id field in struct initializers`
- 2 min: `FFmpeg development headers missing (cannot install without root)`
- 5 min: `fullSessionMarathonStress.test.ts hangs indefinitely`

Attempt 2:

- 2 min: `Missing @tailwindcss/oxide-linux-x64-gnu native binary (npm optional dependency bug)`
- 5 min: `jsdom v29 requires Node 20+ (crypto.hash, ESM require failures)`
- 1 min: `Missing @testing-library/dom needed by @testing-library/react v16`
- `Rust compiler not available - cannot build Tauri backend`
- `Vite 7 requires Node 20.19+ - cannot start dev server or build`
- `Missing FFmpeg development headers (libavformat-dev etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
