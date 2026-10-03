# Pulse

**Verdict: runs.** Argusic Score 97.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rcourtman/Pulse, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/pulse

## Pinned environment

- Project commit: `b3bbf23f082e89b0703909fcb3349387822dd0c1`
- Test commit: `b3bbf23f082e89b0703909fcb3349387822dd0c1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 38.7 to 56.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/37b69f72-bc02-4957-ad43-6b497312c1b6) |
| 2 | pass | 100 | 25 | 38.7 | 2 | 2 | [run](https://argusic.com/run/e21dde18-be00-4456-a080-785200196365) |
| 3 | pass | 95 | 8 | 56.9 | 4 | 3 | [run](https://argusic.com/run/b41b8d22-03c4-44a5-81de-c3e73d06eeeb) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `TestGetDeploymentType_Manual and 3 other tests in internal/updates fail inside Docker environment because isDockerEnvironment() detects /.dockerenv and returns 'docker' instead of expected values`
- `Two repoctl tests (TestStatusJSONLaneEvidenceReferencesAreStructured, TestStatusJSONReadinessAssertionsAreTypedRecords) require sister repos at /work/pulse-pro and /work/pulse-enterprise not present in this container`

Attempt 3:

- 2 min: `Go toolchain not found on system`
- 1 min: `Frontend embed dir frontend-modern/dist empty , Go build fails`
- 1 min: `TestGetDeploymentType_Manual fails inside a Docker container because isDockerEnvironment() sees /.dockerenv`
- `TestStatusJSONLaneEvidenceReferencesAreStructured and TestStatusJSONReadinessAssertionsAreTypedRecords in internal/repoctl require companion repos (pulse-pro, pulse-enterprise) that are absent`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
