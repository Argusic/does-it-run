# extractor

**Verdict: runs with mocks.** Argusic Score 72 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lightfeed/extractor, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/extractor

## Pinned environment

- Project commit: `c9edd2bf363e1c4b03e3c2ea144458ab719cd099`
- Test commit: `c9edd2bf363e1c4b03e3c2ea144458ab719cd099`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 39.2 to 39.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 0.1 | 39.2 | 1 | 0 | [run](https://argusic.com/run/96bbfb52-4f95-43ac-b4e9-dbd894137e84) |

## What was observed on a clean machine

Attempt 1:

- `Playwright MCP bundle requires Node 20+ ESM VM API (Node 18 present) - browser-extraction tests fail at import`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
