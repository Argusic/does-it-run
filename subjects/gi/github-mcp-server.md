# github-mcp-server

**Verdict: runs.** Argusic Score 94.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/github/github-mcp-server, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/github-mcp-server

## Pinned environment

- Project commit: `bd47e638b8c16f780e4b277b5cc5e9ba366efba5`
- Test commit: `bd47e638b8c16f780e4b277b5cc5e9ba366efba5`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 6.6 to 19.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 19.9 | 0 | 0 | [run](https://argusic.com/run/ae905d2e-facc-4c18-a71b-e3d0746a6bdc) |
| 2 | pass with mocks | 92 | 2 | 9.7 | 2 | 2 | [run](https://argusic.com/run/91f7c5e9-3f9a-48ff-900e-a4f32201f9c5) |
| 3 | pass | 100 | 20 | 6.6 | 0 | 0 | [run](https://argusic.com/run/30b343db-53ee-4f8e-802b-313ef2a2e630) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go 1.25.12 not installed in container`
- 1 min: `UI build fails: Node.js v18.19.1 too old (requires >=20.19.0); vite/rolldown imports node:util styleText not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
