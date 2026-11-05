# flowgram.ai

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bytedance/flowgram.ai, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/flowgram-ai

## Pinned environment

- Project commit: `ba1a9630f80263a196d31993cd85fd1c873d9ddd`
- Test commit: `ba1a9630f80263a196d31993cd85fd1c873d9ddd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.4 to 29.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 15.4 | 1 | 1 | [run](https://argusic.com/run/b5eaab9f-f472-4a11-9be9-f530aabfa02d) |
| 2 | pass | 100 | 7.3 | 29.4 | 6 | 6 | [run](https://argusic.com/run/ee0bbd3f-7d16-450d-9041-9046844df3a2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 does not satisfy required range >=18.20.3 <19.0.0 || >=20.14.0 <23.0.0`

Attempt 2:

- 3 min: `Rush requires Node >=18.20.3 but container had 18.19.1 (no root, no nvm); rush was not installed`
- 5 min: `rush test failed in @flowgram.ai/free-layout-editor: unhandled ReferenceError: document is not defined , free-stack-plugin StackingContextManager debounced _compute fired after jsdom teardown`
- 0.8 min: `Playwright didn't ship browsers: chromium_headless_shell-1194 missing`
- 4 min: `fixed-layout e2e failed wholesale (8 failed) when it silently reused the running demo server on port 3000; its webServer runs 'rush', which is not on PATH; and Playwright had run with --update-snapshots before chromium existed`
- `Cosmetic: rsbuild dev --open fails spawn xdg-open ENOENT (no desktop opener in container); server itself stays up`
- 1 min: `runtime-js 'should handle network error' prints a stack from a mocked fetch rejection (HTTPExecutor.execute line 36 trace via retry loop) although the test passes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
