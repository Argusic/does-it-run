# Conduit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ConduitPlatform/Conduit, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/conduit

## Pinned environment

- Project commit: `368a96bc509c9d6052e48ee567462e7c260443e4`
- Test commit: `368a96bc509c9d6052e48ee567462e7c260443e4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10 to 10 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 10 | 5 | 5 | [run](https://argusic.com/run/ab01bd14-5c63-4cec-ace4-d787a9224dd7) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `container had no pnpm/protoc and only Node 18 (repo needs Node>=24, pnpm 11.5.0, protoc 29.x)`
- 2 min: `no redis/mongodb binaries in container`
- 3 min: `pnpm install --frozen-lockfile ran prepare scripts before workspace deps were built, failing chat's tsc (missing @conduitplatform/grpc-sdk types)`
- 2 min: `gRPC PERMISSION_DENIED 'No gRPC protection token provided' when running Core without GRPC_KEY`
- 1 min: `logins 401 'Invalid login credentials' and router 404 for /authentication/local/signup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
