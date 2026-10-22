# vibe-check-mcp-server

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PV-Bhat/vibe-check-mcp-server, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vibe-check-mcp-server

## Pinned environment

- Project commit: `ed8452f2d626011526b0c62f7be7d0a6f67794c1`
- Test commit: `ed8452f2d626011526b0c62f7be7d0a6f67794c1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16 to 16 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 16 | 3 | 3 | [run](https://argusic.com/run/6ca7ca06-af26-4e27-9180-32758c030eb1) |

## What was observed on a clean machine

Attempt 1:

- 7 min: `Container ships Node v18.19.1 but project requires >=20; vitest 4 crashed on node:util.styleText (rolldown bundler) and npm 9 missed the @rolldown/binding-linux-x64-gnu optional dependency, so the build/tests could not run`
- 6 min: `HTTP transport only answered the first request; every subsequent POST to /mcp returned HTTP 500 because the SDK stateless streamable transport throws 'Stateless transport cannot be reused across requests' when one instance is reused`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
