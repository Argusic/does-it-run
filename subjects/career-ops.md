# career-ops

**Verdict: runs.** Argusic Score 98.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/santifer/career-ops, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/career-ops

## Pinned environment

- Project commit: `619a834dd7868092d8faa8a83add3b2c7afc6298`
- Test commits: `619a834dd7868092d8faa8a83add3b2c7afc6298`, `1696bec4d021768e7359f9aad6b329cba883da20`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 6; wall time 24.6 to 65.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 37.1 | 3 | 3 | [run](https://argusic.com/run/f62d82dd-eba5-43bf-8bc7-1995e90a6c57) |
| 1 | pass | 100 | 12 | 32.2 | 3 | 3 | [run](https://argusic.com/run/e281ae56-cdbd-4a0a-b25d-2cd386f5f41b) |
| 2 | pass | 100 | 23 | 24.6 | 5 | 5 | [run](https://argusic.com/run/98db1d40-6add-41d5-8bce-9b080e39a357) |
| 2 | pass | 100 | 55 | 32.3 | 4 | 4 | [run](https://argusic.com/run/c0597d4a-13bc-4dde-b9cd-c617d4792bb3) |
| 3 | pass | 100 | 6 | 65.7 | 3 | 3 | [run](https://argusic.com/run/e8457037-a1e4-4592-a039-a744fed6fddf) |
| 3 | pass | 100 | 36 | 34.7 | 5 | 5 | [run](https://argusic.com/run/1bee7030-8ea2-457f-af5a-93c51abba0c4) |

## What was observed on a clean machine

Attempt 1:

- `node:sqlite not available (needs Node 22+, have 18.19.1) , 5 test failures in tracker SQLite tests`
- `Playwright system library dependencies missing (libnss3, libnspr4, etc.) , PDF generation cannot launch`
- 3 min: `npm install postinstall failed , Playwright 1.62.1 requires Node 20+`

Attempt 1:

- 3 min: `npm install failed because postinstall requires Node 20+ for Playwright, and also fails on Node 20+ because --with-deps needs root`
- 4 min: `node:sqlite not available (tracker tests failed) on Node 18`
- 2 min: `validate-untrusted-content-coverage.mjs uses globSync() from fs (Node 22+ only) , Node 18/20 lacked it`

Attempt 2:

- 2 min: `Playwright requires Node >=20 but container has Node 18`
- 1 min: `npm postinstall fails because playwright install --with-deps needs root for system packages`
- 3 min: `node:sqlite built-in module not available without --experimental-sqlite flag on Node 20/22/23`
- 2 min: `Web tests import .ts files directly and fail on ERR_UNKNOWN_FILE_EXTENSION`
- 1 min: `Experimental feature warnings pollute stderr, causing test assertions to fail on empty-stderr checks`

Attempt 2:

- 5 min: `Node.js v18 is below the minimum for Playwright 1.62.1 (node:sqlite requires 22.5+)`
- 8 min: `npm install postinstall fails: playwright install --with-deps needs root for apt system deps`
- 2 min: `validate-untrusted-content-coverage.mjs uses fs.globSync which requires Node 22+`
- 5 min: `test-all.mjs's web test runner invokes node --test on .mjs files that import .ts sources without --experimental-strip-types`

Attempt 3:

- 2 min: `Node.js 18.19.1 shipped by the container is too old , Playwright 1.62.1 requires Node >=20, and node:sqlite (used by tracker.mjs) requires Node >=22.5`
- 2 min: `npm postinstall script tries to install Playwright Chromium with system dependencies (sudo) and fails because the container has no root access`
- `web/tests/lib/apply-cv-resolver.test.mjs imports .ts files via Node's ESM loader but web/package.json lacks "type": "module", and the runner does not pass --experimental-strip-types`

Attempt 3:

- 2 min: `Node v18 too old (need >=20 for Playwright)`
- 3 min: `npm postinstall failed: --with-deps tries su (no root)`
- 3 min: `node:sqlite unavailable (needs Node >=22.5)`
- 1 min: `validate-untrusted-content-coverage.mjs crashed: globSync missing`
- 5 min: `Web test explore-ai-dedup.test.mjs crashed: cannot import .ts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
