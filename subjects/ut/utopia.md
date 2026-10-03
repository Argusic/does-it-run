# utopia

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deeplethe/utopia, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/utopia

## Pinned environment

- Project commit: `417b49bc44336422d35f68ee3b6bc8ecdfc3e6bb`
- Test commit: `417b49bc44336422d35f68ee3b6bc8ecdfc3e6bb`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 16.9 to 28 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 28 | 4 | 4 | [run](https://argusic.com/run/63f75f48-da68-4b2c-8031-37ed9fb924fd) |
| 2 | pass | 100 | 23 | 16.9 | 0 | 0 | [run](https://argusic.com/run/efe6ebbe-b16f-4c7d-ad15-74a1602a1413) |
| 3 | pass | 100 | 24 | 26.3 | 6 | 6 | [run](https://argusic.com/run/422d27ec-0a39-45f7-8db5-fdcc20c3f8fc) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `No C compiler (cc/gcc) found in container`
- 2 min: `No pkg-config found in container`
- 5 min: `No PostgreSQL or Docker available`
- 3 min: `PostgreSQL segfaulted with shared_preload_libraries = 'vector'`

Attempt 3:

- 1 min: `rustc/cargo not found in PATH`
- 1 min: `pnpm not found`
- 5 min: `PostgreSQL 16 with pgvector not installed (no root)`
- 2 min: `pgvector.so segfaulted on shared_preload_libraries`
- 2 min: `Web frontend build failed: missing @tailwindcss/oxide-linux-x64-gnu native binding (pnpm skipped optional deps)`
- `IPv6 loopback bind failed (os error 99)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
