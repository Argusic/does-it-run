# commerce

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vercel/commerce, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/commerce

## Pinned environment

- Project commit: `3761e52e60df9c6a316e067dbfd7032e494d3634`
- Test commit: `3761e52e60df9c6a316e067dbfd7032e494d3634`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.5 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 8.5 | 4 | 4 | [run](https://argusic.com/run/5abb2251-6525-405c-aa88-014fb867165a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js 18.19.1 is too old for Next.js 15.6 (requires >=20.9.0)`
- 1 min: `pnpm install blocked build scripts (sharp)`
- 5 min: `Shopify GraphQL API requires real credentials; build fails with UNAUTHORIZED`
- 2 min: `Mock server query matching incorrectly handled getProducts vs getProduct and getPages vs getPage`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
