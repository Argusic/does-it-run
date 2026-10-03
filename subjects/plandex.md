# plandex

**Verdict: runs.** Argusic Score 98.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/plandex-ai/plandex, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/plandex

## Pinned environment

- Project commit: `e2d772072efadbe41d2946d97d79be55532dbab5`
- Test commit: `e2d772072efadbe41d2946d97d79be55532dbab5`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 17.9 to 39.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 38 | 39.1 | 6 | 6 | [run](https://argusic.com/run/662fbb1e-8a6a-402b-81aa-67d096327f32) |
| 2 | pass | 100 | 30 | 29.8 | 5 | 5 | [run](https://argusic.com/run/ceda43fb-3089-4979-80a7-d6a4d8569f22) |
| 3 | pass | 96 | 10 | 17.9 | 5 | 4 | [run](https://argusic.com/run/33ea3ac4-cc82-47a3-98e9-4f746c1b6eeb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go not installed`
- 10 min: `No C compiler for tree-sitter CGo dependency (gcc not installable via apt without root)`
- 12 min: `PostgreSQL not installed`
- 5 min: `Python packages for LiteLLM proxy not installed`
- 2 min: `LiteLLM proxy could not find litellm_proxy.py module`
- 1 min: `Migration directory not found at startup`

Attempt 2:

- 3 min: `Go not installed`
- 5 min: `PostgreSQL not installed`
- 2 min: `Python modules uvicorn/fastapi missing`
- 5 min: `uuid-ossp extension dependencies missing`
- 1 min: `Migration dirty state after first uuid-ossp failure`

Attempt 3:

- 1 min: `Go 1.23.3 not pre-installed , installed from official tarball`
- 2 min: `PostgreSQL not installed , used embedded-postgres-binaries JAR`
- 2 min: `Python dependencies uvicorn, fastapi, litellm not installed`
- 2 min: `Server panicked on startup because MIGRATIONS_DIR default is relative and LITELLM_PROXY_DIR not set`
- `less pager not found for CLI paging output`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
