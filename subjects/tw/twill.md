# twill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/area17/twill, licensed Apache-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/twill

## Pinned environment

- Project commit: `d763dee5b60109ee38f83806e478e9c4a2ac36d5`
- Test commit: `d763dee5b60109ee38f83806e478e9c4a2ac36d5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.2 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 10.2 | 5 | 5 | [run](https://argusic.com/run/db498bf8-5cf3-43c2-afee-8fb3123cc168) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP 8.x missing from container`
- `Composer missing from container`
- `MySQL not available for integration tests (DB_CONNECTION=mysql in phpunit.xml)`
- `PermissionsTest fails with SQLite: uses MySQL-only SET FOREIGN_KEY_CHECKS=0;`
- `Paratest parallel execution fails on shared SQLite file due to race conditions`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
