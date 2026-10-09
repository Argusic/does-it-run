# next-wp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/9d8dev/next-wp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/next-wp

## Pinned environment

- Project commit: `4a2caeb1e14191fe58113b94326c2ad92106ff8b`
- Test commit: `4a2caeb1e14191fe58113b94326c2ad92106ff8b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.25 | 5 | 3 | 3 | [run](https://argusic.com/run/97def588-7887-4183-8433-ede7f53c0f99) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pnpm not installed - required Node.js >=22.13 but system had v18.19.1`
- 0.5 min: `corepack signature verification failed trying to download pnpm`
- 3 min: `Turbopack dev server fails with 'Too many open files' due to container file descriptor limit (4096)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
