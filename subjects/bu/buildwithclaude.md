# buildwithclaude

**Verdict: runs with mocks.** Argusic Score 84 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/davepoon/buildwithclaude, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/buildwithclaude

## Pinned environment

- Project commit: `18e6760b99012bac033ff203a988da650cfee0a0`
- Test commit: `18e6760b99012bac033ff203a988da650cfee0a0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 11.1 to 55.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 76 | 6 | 11.1 | 5 | 1 | [run](https://argusic.com/run/f53cd0cf-16a8-49e1-968e-4940eab4d05d) |
| 2 | pass with mocks | 92 | 2 | 55.9 | 3 | 3 | [run](https://argusic.com/run/80a15d47-f020-4f89-9401-464943003caf) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `package.json test:unit script uses --experimental-strip-types which Node 18 doesn't support`
- 3 min: `scripts/generate-registry.js requires fetch-docker-mcp.js, fetch-official-mcp.js, enhance-docker-stats.js , none exist in the repo`
- `mcp-servers/ directory referenced by generate-registry.js but does not exist`
- 2 min: `Next.js 16 build requires Node >=20.9.0, environment has Node 18.19.1 , web-ui cannot build`
- `npm install had 11 EBADENGINE warnings for Node 18 vs required Node 20+ for several packages`

Attempt 2:

- 2 min: `web-ui unit tests failed under the container Node 18 with 'bad option: --experimental-strip-types'`
- 3 min: `web-ui/server.js did not exist at the repo root (standalone output lives at web-ui/.next/standalone/web-ui/server.js)`
- 20 min: `DB-backed pages logged 127.0.0.1:5432 connection failures and the server exited after /skills; a local Postgres-protocol stub accepts TCP but postgres-js still times out mid-handshake`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
