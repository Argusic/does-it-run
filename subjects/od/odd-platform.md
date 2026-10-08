# odd-platform

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/opendatadiscovery/odd-platform, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/odd-platform

## Pinned environment

- Project commit: `015f6fa2dac9b6d0dfd00b6b6d9baab9329e6c4f`
- Test commit: `015f6fa2dac9b6d0dfd00b6b6d9baab9329e6c4f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.9 to 23.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 23.9 | 8 | 8 | [run](https://argusic.com/run/25bc748b-151f-407d-a65f-92ec96f9e203) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Java 17 (JDK) not found in the container`
- 2 min: `Docker not available , JOOQ codegen (jooqDockerGenerate task) uses Testcontainers which needs Docker`
- 5 min: `PostgreSQL not installed; needed for both JOOQ codegen and runtime`
- 2 min: `Node.js 24+ required by frontend but only v18.19.1 was available`
- 1 min: `pnpm (required by frontend) not found, npm install -g failed due to permissions`
- 2 min: `Frontend generate.sh uses Docker to run openapi-generator-cli`
- `317/962 backend tests fail because Testcontainers needs Docker`
- `12/384 frontend tests fail with pre-existing TypeScript type mismatches in generated-sources`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
