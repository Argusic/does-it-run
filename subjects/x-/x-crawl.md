# x-crawl

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coder-hxl/x-crawl, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/x-crawl

## Pinned environment

- Project commit: `0c8d0c8c51b8d2d8864f789bae8d17e1ba360c0a`
- Test commit: `0c8d0c8c51b8d2d8864f789bae8d17e1ba360c0a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 34 to 34 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17 | 34 | 4 | 4 | [run](https://argusic.com/run/c7a38d9a-2662-44d6-ad17-57b51d85f435) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Node.js 18.19.1 is below the project's requirement (>=24.16.0). vitest runner fails with 'SyntaxError: Unexpected token with' because Node 18 does not support the 'with { type: 'json' }' import attribute that vite/vitest emit.`
- 3 min: `TypeScript build error: 'CookieParam' type from devtools-protocol incompatible with puppeteer-core's 'CookieParam' (partitionKey.sourceOrigin missing)`
- 1 min: `TypeScript build error: 'PuppeteerLaunchOptions' export renamed to 'LaunchOptions' in puppeteer v24`
- 3 min: `vitest 3.2.4 and @vitest/coverage-v8 3.2.6 version mismatch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
