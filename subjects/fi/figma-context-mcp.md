# Figma-Context-MCP

**Verdict: runs.** Argusic Score 94.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GLips/Figma-Context-MCP, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/figma-context-mcp

## Pinned environment

- Project commit: `c083d65c7e002923e7cb98f4e3bdafb105e90f6d`
- Test commit: `c083d65c7e002923e7cb98f4e3bdafb105e90f6d`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 3.1 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass with mocks | 92 | 2 | 8.1 | 1 | 1 | [run](https://argusic.com/run/0ff0d6af-221e-448e-8edc-98f4e9881620) |
| 2 | pass | 100 | 6.2 | 3.6 | 3 | 3 | [run](https://argusic.com/run/ed1434ac-4774-4eee-bd83-e900c0b26988) |
| 3 | pass with mocks | 92 | 3 | 3.1 | 4 | 4 | [run](https://argusic.com/run/f74c7c08-995a-488b-847a-4c505202f9c0) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js v18 is installed but project requires >=20.20.0`

Attempt 2:

- 1.5 min: `Node.js v18.19.1 installed but project requires >=20.20.0`
- 0.2 min: `.npmrc set prefix=/home/runner/.npm-global but the directory did not exist, causing npm install errors`
- 0.5 min: `pnpm not available in system`

Attempt 3:

- 1 min: `pnpm not found`
- 3 min: `Node.js v18.19.1 too old (needs >=20.20.0) , undici@7 requires File global`
- 1 min: `EACCES installing global corepack`
- 1 min: `n failed to write to /usr/local/n (EACCES)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
