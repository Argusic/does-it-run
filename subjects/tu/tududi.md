# tududi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chrisvel/tududi, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/tududi

## Pinned environment

- Project commit: `7f5da6d152115265cd2a60ae827d0c967e67eebc`
- Test commit: `7f5da6d152115265cd2a60ae827d0c967e67eebc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 80.1 to 80.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 80.1 | 2 | 2 | [run](https://argusic.com/run/80bf8e50-2781-4100-b697-f276750c677d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `jose v6 is ESM-only, cannot be require()d by oidc/service.js on Node 18`
- 2 min: `MCP SDK CJS output uses globalThis.crypto.randomUUID() which is undefined on Node 18 without --experimental-global-webcrypto`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
