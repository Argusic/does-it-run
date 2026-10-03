# mcp-server-cloudflare

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cloudflare/mcp-server-cloudflare, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mcp-server-cloudflare

## Pinned environment

- Project commit: `1d7a16b25db74ed44539cd5079e2db46b42f08db`
- Test commit: `1d7a16b25db74ed44539cd5079e2db46b42f08db`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.5 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 6.5 | 1 | 1 | [run](https://argusic.com/run/2afce454-776c-4dd8-bd17-4030c0ebabbe) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node 18 lacks global File API required by undici/workerd`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
