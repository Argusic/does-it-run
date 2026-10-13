# reddit-mcp-buddy

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/karanb192/reddit-mcp-buddy, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/reddit-mcp-buddy

## Pinned environment

- Project commit: `8d31a285db78d8e34546c1d1023e7550bbc2c135`
- Test commit: `8d31a285db78d8e34546c1d1023e7550bbc2c135`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 21.8 to 21.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 21.8 | 3 | 3 | [run](https://argusic.com/run/c21d7a98-5f0e-4b99-9c7b-d1aa6112738c) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `Reddit API/token URLs are hardcoded (src/core/auth.ts, src/services/reddit-api.ts), so the app cannot be pointed at a mock without a source change`
- 3 min: `Node 18 fetch ignores HTTPS_PROXY/HTTP_PROXY by design, so env-proxy mocking of the hardcoded https://www.reddit.com token endpoint failed`
- 1 min: `Anonymous live Reddit access is rate-limited/blocked from this container (403/429), so credential-gated integration tests were skipped by the suite`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
