# nanobrowser

**Verdict: runs.** Argusic Score 90.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nanobrowser/nanobrowser, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nanobrowser

## Pinned environment

- Project commit: `24a14b76e14a9c30fd84878ca7985049d1e7d064`
- Test commit: `24a14b76e14a9c30fd84878ca7985049d1e7d064`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services, real run
- Valid runs: 3; wall time 14.7 to 17 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 26 | 14.7 | 4 | 4 | [run](https://argusic.com/run/1249f04b-a84a-4050-936c-efc41d15e3f6) |
| 2 | pass with mocks | 92 | 8 | 17 | 4 | 4 | [run](https://argusic.com/run/c3e3be4a-a46c-4f75-b088-918a4caca7fc) |
| 3 | pass | 100 | 14.8 | 15.4 | 2 | 2 | [run](https://argusic.com/run/6465782d-837f-45fb-8b05-dfef2d99ecfb) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 does not meet engine requirement >=22.12.0`
- 1 min: `pnpm not found (required package manager)`
- 1 min: `packages/schema-utils/index.ts exports non-existent ./lib/json_gemini and ./lib/helpers modules`

Attempt 2:

- 1 min: `Node.js v18.19.1 installed but package requires >=22.12.0`
- 1 min: `pnpm not found; npm install globally failed due to permissions`
- 1 min: `packages/schema-utils/index.ts exports non-existent modules ./lib/json_gemini and ./lib/helpers`

Attempt 3:

- 3 min: `packages/schema-utils/index.ts exported non-existent modules './lib/json_gemini' and './lib/helpers' which don't exist in lib/`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
