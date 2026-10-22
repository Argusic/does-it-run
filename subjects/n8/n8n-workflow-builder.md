# n8n-workflow-builder

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/makafeli/n8n-workflow-builder, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/n8n-workflow-builder

## Pinned environment

- Project commit: `411c0a75f512898572c3de80f86d5b5c3939f041`
- Test commit: `411c0a75f512898572c3de80f86d5b5c3939f041`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.5 to 4.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.5 | 4.5 | 1 | 1 | [run](https://argusic.com/run/9c08e909-ebf4-40c2-854d-7eb4d15f8b18) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `16 tests failed: MCPTestClient mock returned hardcoded success without calling axios, so error-path tests that mocked axios to reject never got isError=true`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
