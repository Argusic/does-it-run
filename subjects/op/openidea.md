# openidea

**Verdict: runs.** Argusic Score 91.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/l0ng-ai/openidea, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openidea

## Pinned environment

- Project commit: `429e8ffc829531d5e5af3a1c03deb969ab0f388a`
- Test commit: `429e8ffc829531d5e5af3a1c03deb969ab0f388a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 21.2 to 30.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 87 | 18 | 30.8 | 4 | 3 | [run](https://argusic.com/run/2079c9fb-eafc-46f9-a84e-ac84623adbb0) |
| 2 | pass | 96 | 21 | 21.2 | 5 | 4 | [run](https://argusic.com/run/72a29422-75b1-46a8-8862-9f6e2a105b1b) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pnpm, cargo and rustc were missing and Node was 18 (README requires Node 22)`
- 1 min: `Playwright browsers missing; --with-deps requires root`
- 11 min: `Default 2-worker e2e run: 16/22 tests timed out during shared goto('/') fixture while the app rendered fine`
- 3 min: `Tauri desktop shell cannot compile: glib-2.0.pc and webkit2gtk-4.1 dev files absent and no root to install them`

Attempt 2:

- 1 min: `pnpm not found in environment`
- 9 min: `Rust toolchain (rustc/cargo) not found`
- 3 min: `Node.js v18 too old for vitest/rolldown v8 (needs styleText from util)`
- 1 min: `Rolldown native binding missing after Node version switch`
- `Tauri desktop shell (src-tauri) cannot build: missing system dev packages libwebkit2gtk-4.1-dev and libglib2.0-dev (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
