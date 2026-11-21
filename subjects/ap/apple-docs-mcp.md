# apple-docs-mcp

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kimsungwhee/apple-docs-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/apple-docs-mcp

## Pinned environment

- Project commit: `28c06cbaa896cb4f89239d30cb20152a74c78cdb`
- Test commit: `28c06cbaa896cb4f89239d30cb20152a74c78cdb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 4.3 to 9.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.3 | 1 | 1 | [run](https://argusic.com/run/ae46777b-71f5-46aa-906c-eb48fefebce2) |
| 2 | pass with mocks | 92 | 0.1 | 9.2 | 1 | 1 | [run](https://argusic.com/run/92664d3d-5e33-4817-9036-1fedd625e401) |

## What was observed on a clean machine

Attempt 1:

- 13 min: `undici@7.16.0 (dep of cheerio@1.1.2) references global 'File' class only available in Node 20+, but Node 18.19.1 is installed`

Attempt 2:

- 5 min: `Node.js 18 lacks global File constructor needed by undici 7.x (pulled by cheerio)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
