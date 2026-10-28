# jev-review

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NiazMorshed2007/jev-review, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/jev-review

## Pinned environment

- Project commit: `57690af54ef7d862c2483342c1e61c14dffcf727`
- Test commit: `57690af54ef7d862c2483342c1e61c14dffcf727`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.6 to 7.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 7.6 | 2 | 2 | [run](https://argusic.com/run/28015180-a9b5-494d-bcb0-04195b8f69cb) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `npm test failed: 'node --test .test-dist/test/**/*.test.js' matched no files because the double-star glob is not expanded and Node 20's --test treats the literal '**' as a filename`
- 2 min: `Container Node is v18.19.1 but the project requires Node 20+ (engines and esbuild target node20); cannot install system packages without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
