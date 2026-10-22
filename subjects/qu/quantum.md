# Quantum

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rodyherrera/Quantum, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/quantum

## Pinned environment

- Project commit: `fe6f89fc24e5c68e10aad6e6c6307eaa5e3b09f6`
- Test commit: `fe6f89fc24e5c68e10aad6e6c6307eaa5e3b09f6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.9 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 5.5 | 5.9 | 4 | 3 | [run](https://argusic.com/run/1269f841-6cce-4570-8f21-37d303fd9c79) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm 12 blocked postinstall build scripts (esbuild etc.)`
- 3 min: `API test suite failed: role quantum does not exist and missing test database`
- 0.5 min: `api start failed on Config::MissingEnv DOMAIN/CLIENT_HOST`
- `4 of 45 API test files failed waiting for Request::ValidationFailed on oversized/empty body`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
