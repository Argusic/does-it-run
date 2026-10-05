# DevDocs

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cyberagiinc/DevDocs, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/devdocs

## Pinned environment

- Project commit: `f8fa9de505c96bcc8c76561196a75d39b52847b6`
- Test commit: `f8fa9de505c96bcc8c76561196a75d39b52847b6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 22.8 to 22.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 22.8 | 3 | 3 | [run](https://argusic.com/run/1364c1ed-c440-4d77-9a85-79bf26f1694d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Python packages cannot be installed system-wide due to externally-managed-environment (PEP 668)`
- 3 min: `Backend depends on external crawl4ai Docker container at http://crawl4ai:11235 for crawling operations`
- 1 min: `Frontend .env file had a malformed concatenated line (DISCOVERY_POLLING_TIMEOUT_SECONDS=300BACKEND_URL=...) and no NEXT_PUBLIC_BACKEND_URL`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
