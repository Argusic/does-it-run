# career-ops

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/santifer/career-ops, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/run/f62d82dd-eba5-43bf-8bc7-1995e90a6c57

## Pinned environment

- Project commit: `619a834dd7868092d8faa8a83add3b2c7afc6298`
- Test commit: `619a834dd7868092d8faa8a83add3b2c7afc6298`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 24.6 to 37.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 37.1 | 3 | 3 | [run](https://argusic.com/run/f62d82dd-eba5-43bf-8bc7-1995e90a6c57) |
| 2 | pass | 100 | 23 | 24.6 | 5 | 5 | [run](https://argusic.com/run/98db1d40-6add-41d5-8bce-9b080e39a357) |
| 3 | pass | 100 | 36 | 34.7 | 5 | 5 | [run](https://argusic.com/run/1bee7030-8ea2-457f-af5a-93c51abba0c4) |

## What was observed on a clean machine

Attempt 1:

- `node:sqlite not available (needs Node 22+, have 18.19.1) , 5 test failures in tracker SQLite tests`
- `Playwright system library dependencies missing (libnss3, libnspr4, etc.) , PDF generation cannot launch`
- 3 min: `npm install postinstall failed , Playwright 1.62.1 requires Node 20+`

Attempt 2:

- 2 min: `Playwright requires Node >=20 but container has Node 18`
- 1 min: `npm postinstall fails because playwright install --with-deps needs root for system packages`
- 3 min: `node:sqlite built-in module not available without --experimental-sqlite flag on Node 20/22/23`
- 2 min: `Web tests import .ts files directly and fail on ERR_UNKNOWN_FILE_EXTENSION`
- 1 min: `Experimental feature warnings pollute stderr, causing test assertions to fail on empty-stderr checks`

Attempt 3:

- 2 min: `Node v18 too old (need >=20 for Playwright)`
- 3 min: `npm postinstall failed: --with-deps tries su (no root)`
- 3 min: `node:sqlite unavailable (needs Node >=22.5)`
- 1 min: `validate-untrusted-content-coverage.mjs crashed: globSync missing`
- 5 min: `Web test explore-ai-dedup.test.mjs crashed: cannot import .ts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
