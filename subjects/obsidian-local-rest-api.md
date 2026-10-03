# obsidian-local-rest-api

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coddingtonbear/obsidian-local-rest-api, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/obsidian-local-rest-api

## Pinned environment

- Project commit: `0278df908a9112d3e694f94c02f196f101dc095a`
- Test commit: `0278df908a9112d3e694f94c02f196f101dc095a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.8 to 16.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 2 | 16.8 | 2 | 1 | [run](https://argusic.com/run/1674d3ba-95f4-44fd-b3bd-2c004b8efb84) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `6 certificates tests failed: SSL routines::ee key too small (RSA 1024-bit keys rejected by OpenSSL 3.0 on Node 18)`
- 2 min: `mcpSessionfulClient test fails: pkce-challenge requires ESM VM API unsupported by Node 18 (project requires >=22)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
