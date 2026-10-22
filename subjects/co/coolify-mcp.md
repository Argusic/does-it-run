# coolify-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/StuMason/coolify-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/coolify-mcp

## Pinned environment

- Project commit: `a32b0a13bcaabe585e276569ed68bd10dedaa5d7`
- Test commit: `a32b0a13bcaabe585e276569ed68bd10dedaa5d7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.3 to 11.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10.2 | 11.3 | 2 | 2 | [run](https://argusic.com/run/98e35606-2441-4c4b-a0fb-0a608c18b607) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `globalThis.crypto.subtle is undefined in Node 18.19.1 , MCP SDK v2's createRequestStateCodec throws on startup and in tests`
- `3 doctor.test.ts tests fail because they assert runtime status is 'pass', but Node 18 produces 'warn' (expected Node 20+)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
