# caddy-proxy-manager

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ingres-si/caddy-proxy-manager, licensed NOASSERTION, written in TypeScript.

Evidence and recordings: https://argusic.com/run/f1a7a80b-1a6c-4852-9d98-e8d41c72db9d

## Pinned environment

- Project commit: `c1a06f3216c412abf4a6275bd5fab76d1fb70a7c`
- Test commit: `c1a06f3216c412abf4a6275bd5fab76d1fb70a7c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.8 to 23.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 23.8 | 5 | 5 | [run](https://argusic.com/run/f1a7a80b-1a6c-4852-9d98-e8d41c72db9d) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18 lacks styleText export needed by rolldown/vitest`
- 2 min: `rolldown native binding missing after first npm install with wrong Node version`
- 8 min: `next build OOM during TypeScript type checking (90 workers)`
- 2 min: `Server bound to container hostname instead of 0.0.0.0, not reachable`
- `Pre-existing test failure: maplibre-gl v6 worker no longer imports maplibre-gl-shared.mjs by relative path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
