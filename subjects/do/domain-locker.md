# domain-locker

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lissy93/domain-locker, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/domain-locker

## Pinned environment

- Project commit: `65eb45d2e4a438132946dcb4cd4f753088f970ab`
- Test commit: `65eb45d2e4a438132946dcb4cd4f753088f970ab`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 8.7 to 15.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 15.3 | 3 | 3 | [run](https://argusic.com/run/3cf70fa2-e81e-452c-a98f-14a927cc03eb) |
| 2 | pass | 100 | 5.5 | 8.7 | 1 | 1 | [run](https://argusic.com/run/66ebc4b8-9c58-4da9-90d1-84cb0f288ad2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js version too old (v18.19.1, needed >=20)`
- 3 min: `Yarn not installed and engine constraint blocked install`
- 1 min: `npm .npmrc prefix config conflicted with nvm`

Attempt 2:

- 2.5 min: `Node version mismatch: container had v18.19.1 but project requires >=20.0.0 (engine-strict=true in .npmrc)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
