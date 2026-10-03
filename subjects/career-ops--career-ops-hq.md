# career-ops

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/career-ops-hq/career-ops, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/run/e281ae56-cdbd-4a0a-b25d-2cd386f5f41b

## Pinned environment

- Project commit: `1696bec4d021768e7359f9aad6b329cba883da20`
- Test commit: `1696bec4d021768e7359f9aad6b329cba883da20`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 32.2 to 65.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 32.2 | 3 | 3 | [run](https://argusic.com/run/e281ae56-cdbd-4a0a-b25d-2cd386f5f41b) |
| 2 | pass | 100 | 55 | 32.3 | 4 | 4 | [run](https://argusic.com/run/c0597d4a-13bc-4dde-b9cd-c617d4792bb3) |
| 3 | pass | 100 | 6 | 65.7 | 3 | 3 | [run](https://argusic.com/run/e8457037-a1e4-4592-a039-a744fed6fddf) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `npm install failed because postinstall requires Node 20+ for Playwright, and also fails on Node 20+ because --with-deps needs root`
- 4 min: `node:sqlite not available (tracker tests failed) on Node 18`
- 2 min: `validate-untrusted-content-coverage.mjs uses globSync() from fs (Node 22+ only) , Node 18/20 lacked it`

Attempt 2:

- 5 min: `Node.js v18 is below the minimum for Playwright 1.62.1 (node:sqlite requires 22.5+)`
- 8 min: `npm install postinstall fails: playwright install --with-deps needs root for apt system deps`
- 2 min: `validate-untrusted-content-coverage.mjs uses fs.globSync which requires Node 22+`
- 5 min: `test-all.mjs's web test runner invokes node --test on .mjs files that import .ts sources without --experimental-strip-types`

Attempt 3:

- 2 min: `Node.js 18.19.1 shipped by the container is too old , Playwright 1.62.1 requires Node >=20, and node:sqlite (used by tracker.mjs) requires Node >=22.5`
- 2 min: `npm postinstall script tries to install Playwright Chromium with system dependencies (sudo) and fails because the container has no root access`
- `web/tests/lib/apply-cv-resolver.test.mjs imports .ts files via Node's ESM loader but web/package.json lacks "type": "module", and the runner does not pass --experimental-strip-types`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
