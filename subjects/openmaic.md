# OpenMAIC

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/THU-MAIC/OpenMAIC, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openmaic

## Pinned environment

- Project commit: `d4ef5faa7636d507dbfe8e17d69e2aeea9083a58`
- Test commit: `d4ef5faa7636d507dbfe8e17d69e2aeea9083a58`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 26.4 to 43.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 43.3 | 0 | 0 | [run](https://argusic.com/run/20ef70c1-82b9-461d-90a6-df977a469276) |
| 1 | pass | 100 | 25 | 35 | 3 | 3 | [run](https://argusic.com/run/2a07f8e5-d7b0-4bab-a298-e59e8fbde681) |
| 3 | pass | 100 | 21 | 26.4 | 3 | 3 | [run](https://argusic.com/run/b1813ede-dd3b-4ffe-9f13-920cd3c5847e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 was installed but the project requires >=20.9.0. Installed v22.23.2 via n to a user-writable prefix.`
- 1 min: `pnpm was not installed globally. corepack was used to prepare pnpm@10.`
- `12 tests failed out of 7134 total (11 test failures + 9 unhandled worker errors) , all timeouts from resource contention in the parallel test pool, not logic bugs. Each failing file passes when run individually.`

Attempt 3:

- 3 min: `Node.js v18.19.1 installed but project requires >=20.9.0`
- 2 min: `pnpm not available - npm install -g pnpm failed (EACCES)`
- 2 min: `rolldown binding-linux-x64-gnu optional dependency not installed - node_modules missing native binary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
