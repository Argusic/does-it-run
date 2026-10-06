# portabase

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Portabase/portabase, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/portabase

## Pinned environment

- Project commit: `6cb2afdbc09bad0accb1d4e4a384f3bed97d5ad5`
- Test commit: `6cb2afdbc09bad0accb1d4e4a384f3bed97d5ad5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28.8 to 28.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 28.8 | 7 | 7 | [run](https://argusic.com/run/992892e6-65e1-49d5-b1bd-131d3794d386) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pnpm not installed on Node.js 18.19.1`
- 3 min: `Node.js 18 too old for Next.js 16 (requires >=20.9.0)`
- 2 min: `@tailwindcss/oxide native binding not found (pnpm skips optional deps)`
- 1 min: `PROJECT_SECRET env var empty , env validation rejected it`
- 8 min: `PostgreSQL not available in container`
- 2 min: `Database migrations not applied , tables missing`
- 2 min: `Corrupted CSS cache from earlier failed build caused 500 on page render`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
