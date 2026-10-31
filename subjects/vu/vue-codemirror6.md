# vue-codemirror6

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/logue/vue-codemirror6, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vue-codemirror6

## Pinned environment

- Project commit: `1e9fdeba8ebe5f808322d2420ee4df12aaf95f84`
- Test commit: `1e9fdeba8ebe5f808322d2420ee4df12aaf95f84`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3.3 to 3.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6.4 | 3.3 | 2 | 2 | [run](https://argusic.com/run/b28dc065-c692-40a3-a185-b4fb4a5e1bd2) |

## What was observed on a clean machine

Attempt 1:

- 2.2 min: `pnpm test: Unsupported Node.js version: "18.19.1". Expected Node.js >= 20.`
- 2.5 min: `pnpm run build: vize type-check failed: Cannot find native binding.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
