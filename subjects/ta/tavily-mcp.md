# tavily-mcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tavily-ai/tavily-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tavily-mcp

## Pinned environment

- Project commit: `1c1d54c2a619afe52544f775c8d82a56ac6d8bb5`
- Test commit: `1c1d54c2a619afe52544f775c8d82a56ac6d8bb5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.6 to 1.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.2 | 1.7 | 0 | 0 | [run](https://argusic.com/run/0c6a7ad0-4d7e-44f0-b462-a7dee488cd0e) |
| 2 | pass | 100 | 0.15 | 1.6 | 1 | 1 | [run](https://argusic.com/run/ba12cbfe-0a00-4cf0-a7f6-5f3aa6d62d48) |

## What was observed on a clean machine

Attempt 2:

- `npm warns EBADENGINE: @hono/node-server requires Node >=20 but system has v18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
