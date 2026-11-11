# brightdata-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/brightdata/brightdata-mcp, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/brightdata-mcp

## Pinned environment

- Project commit: `d33cfa5da4a294d63a73ef96f0ee1fa90d892741`
- Test commit: `d33cfa5da4a294d63a73ef96f0ee1fa90d892741`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 2.5 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 4.2 | 1 | 1 | [run](https://argusic.com/run/178d3683-76c4-40ad-acf6-913b856cfcd7) |
| 2 | pass with mocks | 92 | 3.5 | 2.5 | 1 | 1 | [run](https://argusic.com/run/2f0aab33-d472-4e47-ba07-f13c54a79263) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `System Node.js v18.19.1 is too old for fastmcp dependency undici (requires >=20.18.1), causing ReferenceError: File is not defined at import`

Attempt 2:

- 1.5 min: `System Node.js 18.19.1 is too old for undici@7.16.0 (transitive dep of fastmcp) which requires Node >= 20 , ReferenceError: File is not defined at webidl/index.js`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
