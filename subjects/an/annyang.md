# annyang

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TalAter/annyang, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/annyang

## Pinned environment

- Project commit: `c31928ac9ae13df13fc7a370530065ea5a7502c1`
- Test commit: `c31928ac9ae13df13fc7a370530065ea5a7502c1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 10.9 to 34.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 10.9 | 1 | 1 | [run](https://argusic.com/run/ef984f05-9627-405e-8159-814a281a16d7) |
| 2 | pass with mocks | 92 | 33 | 34.9 | 4 | 4 | [run](https://argusic.com/run/b351db1f-04bf-4adb-be2b-6e555bdb48f7) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `vitest 4.x requires Node.js >=20 but container has Node v18.19.1; 145 tests failed with hook timeouts`

Attempt 2:

- 2 min: `pnpm not present and global npm install blocked by EACCES on /usr/local`
- 2 min: `pnpm 10 ignored esbuild build script so tsup could not run`
- 15 min: `vitest 4 vi.useRealTimers() in afterEach hung (10s hook timeout) whenever annyang restart timer chains were pending; 145/165 tests failed with Hook timed out`
- 14 min: `3 auto-restart/restart-warning tests exceeded vitest 4 default 5s test timeout while advancing 10k-20k chained fake timer cycles`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
