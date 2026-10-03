# firecrawl-mcp-server

**Verdict: runs.** Argusic Score 90.2 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/firecrawl/firecrawl-mcp-server, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/firecrawl-mcp-server

## Pinned environment

- Project commit: `089748bed6883725f926e922657865b1eb812e27`
- Test commit: `089748bed6883725f926e922657865b1eb812e27`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 4 to 24.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 86.67 | 3 | 24.3 | 3 | 1 | [run](https://argusic.com/run/2861ff44-6a5b-4574-83f0-6473e36cfac7) |
| 2 | pass with mocks | 92 | 1.2 | 4 | 2 | 2 | [run](https://argusic.com/run/6b9e2315-e1a5-49f0-b1a9-53e707f46754) |
| 3 | pass with mocks | 92 | 12 | 9.7 | 2 | 2 | [run](https://argusic.com/run/f33b5311-aa1e-42ea-9e0e-f1d398c924bf) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js v18 installed but project requires >=22; undici dependency crashes on Node 18 with 'File is not defined'`
- `Tests 34/59: keyless HTTP cloud tool listing returns all 25 tools instead of only parse/scrape/search`
- `Test 70: firecrawl_extract deprecated response causing TypeError`

Attempt 2:

- 0.9 min: `Node.js v18 was installed but the project requires >=22`
- 0.2 min: `pnpm not found on PATH`

Attempt 3:

- 6 min: `System Node.js was v18.19.1 but package.json requires >=22; the project also needs pnpm for its fastmcp patch (no pnpm/corepack installed, no root for apt)`
- 2 min: `First headless HTTP launch attempt failed: 'ReferenceError: File is not defined' in undici because the backgrounded process inherited system Node v18 from the shell environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
