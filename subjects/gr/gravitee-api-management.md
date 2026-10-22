# gravitee-api-management

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gravitee-io/gravitee-api-management, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/gravitee-api-management

## Pinned environment

- Project commit: `8e781f91365e4b7f1956f71ad477776bc54a0c74`
- Test commit: `8e781f91365e4b7f1956f71ad477776bc54a0c74`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 37 to 37 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 23 | 37 | 1 | 0 | [run](https://argusic.com/run/0356a3ff-3aa1-45cc-9077-63ce8a5f9029) |

## What was observed on a clean machine

Attempt 1:

- `Maven build missing required enterprise artifacts (com.graviteesource.gamma.module and several io.gravitee.policy packages) for distribution assembly`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
