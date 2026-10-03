# mcp-context-forge

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/IBM/mcp-context-forge, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/mcp-context-forge

## Pinned environment

- Project commit: `1c198de701e813e4b972aafb653e7b0f4990bcb1`
- Test commit: `1c198de701e813e4b972aafb653e7b0f4990bcb1`
- Worker image digests: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`, `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 32.4 to 52.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 8 | 52.2 | 1 | 1 | [run](https://argusic.com/run/ab0ecb1d-b8cc-43a5-bb3a-d15f6d411806) |
| 2 | timeout | none | 3.5 | 47.9 | 0 | 0 | [run](https://argusic.com/run/5a30c4a0-5c52-45f5-bf51-4992c87fc6b9) |
| 2 | pass | 100 | 33 | 32.4 | 2 | 2 | [run](https://argusic.com/run/82fa0ed3-29f4-4888-b32e-abe27e0da0ad) |

## What was observed on a clean machine

Attempt 1:

- `npm engine warnings for Admin UI build (Node 18 vs 20+ required)`

Attempt 2:

- 3 min: `npm build-ui failed: Node.js 18.19.1 too old for Vite 7.x (requires >=20.19.0)`
- 2 min: `make check-env validates .env.example instead of .env, causing false positive failure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
