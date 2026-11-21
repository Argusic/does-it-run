# pintora

**Verdict: runs.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hikerpig/pintora, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pintora

## Pinned environment

- Project commit: `695eb2ed22460bd083808b88b3fdd8fbd03c02df`
- Test commit: `695eb2ed22460bd083808b88b3fdd8fbd03c02df`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.2 to 25.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 25.3 | 2 | 2 | [run](https://argusic.com/run/490f7812-1762-43e9-83db-75e6105030be) |
| 2 | fail | 50 | 2.5 | 6.2 | 5 | 5 | [run](https://argusic.com/run/b7e71f09-d240-4bbc-a30e-0b24f730d62d) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `rolldown requires Node 20+ (node:util/styleText)`
- 6 min: `jsdom@29 dep webidl-conversions@8.0.1 requires Node 20+`

Attempt 2:

- 1 min: `pnpm was not installed in the container`
- 1 min: `pnpm compile failed: @pintora/standalone uses rolldown which needs Node 21+ (styleText from node:util not in Node 18)`
- `CLI render.spec.ts and render-cases.spec.ts fail because jsdom@29 -> webidl-conversions@8 uses ArrayBuffer.prototype.resizable.get() (Node 21+ API not available in Node 18)`
- `rolldown-build.spec.ts (standalone) fails because rolldown build artifacts don't exist on Node 18`
- `CLI binary cannot start because it requires jsdom (imported in render-impl.ts) which crashes on Node 18 at webidl-conversions`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
