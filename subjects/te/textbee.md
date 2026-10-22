# textbee

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/textbee/textbee, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/textbee

## Pinned environment

- Project commit: `454e59e4d059a6d25d385ce292be3b2a799ee7bb`
- Test commit: `454e59e4d059a6d25d385ce292be3b2a799ee7bb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.1 to 24.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 24.1 | 5 | 5 | [run](https://argusic.com/run/a18a6ffc-560b-417a-808a-3bd8db876bf2) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm binary not in PATH`
- 5 min: `API billing webhook tests fail: globalThis.crypto.subtle undefined in ts-jest (polar-sdk v1.0.0 requires Node>=22)`
- 3 min: `Web postcss tailwindcss native binding missing (requires Node>=20)`
- 1 min: `Next.js web build requires Node>=20.9.0 (system has 18.19.1)`
- 1 min: `API NestJS build does not copy mail template assets to dist`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
