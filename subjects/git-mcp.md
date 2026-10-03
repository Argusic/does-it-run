# git-mcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/idosal/git-mcp, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/git-mcp

## Pinned environment

- Project commit: `c487a29895dcfcb5b672247e646426a56e2051c1`
- Test commit: `c487a29895dcfcb5b672247e646426a56e2051c1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 6.6 to 20.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 12.9 | 2 | 2 | [run](https://argusic.com/run/14c254f6-6692-4b23-a0c7-706ab7068aa9) |
| 2 | pass | 100 | 1 | 20.4 | 1 | 1 | [run](https://argusic.com/run/7dcaaf56-6c4a-4e6e-84bb-66d10683b146) |
| 3 | pass | 100 | 10 | 6.6 | 0 | 0 | [run](https://argusic.com/run/fd2d660d-e2b5-4928-9293-144b22fa33c7) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pnpm not installed in container; installed pnpm@10.7.1 globally via npm to user's ~/.npm-local/bin`
- 0.5 min: `Node v18.19.1 detected; react-router dev requires >20, but wrangler dev works with Miniflare`

Attempt 2:

- `Node.js v18 detected but react-router and wrangler recommend v20+`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
