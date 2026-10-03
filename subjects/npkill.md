# npkill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/voidcosmos/npkill, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/npkill

## Pinned environment

- Project commit: `2dad63647fdd6887e9022c8d22887fe5606eb92f`
- Test commit: `2dad63647fdd6887e9022c8d22887fe5606eb92f`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 2 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.98 | 2.6 | 0 | 0 | [run](https://argusic.com/run/5eab5165-4ac5-43c2-8af1-0af480725b01) |
| 2 | pass | 100 | 2 | 3.7 | 1 | 1 | [run](https://argusic.com/run/0dcb13da-677f-49bc-8ddc-36fb3bb7c782) |
| 3 | pass | 100 | 0.3 | 2 | 0 | 0 | [run](https://argusic.com/run/bf968784-5064-44d1-ab4b-ba98ea391415) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Missing devDependency 'tsconfig-paths' caused 'npm run start' to fail with MODULE_NOT_FOUND`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
