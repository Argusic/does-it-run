# js-reverse-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zhizhuodemao/js-reverse-mcp, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/js-reverse-mcp

## Pinned environment

- Project commit: `bf7dc506e8743ba1ec5bd3325c91818b9192e40e`
- Test commit: `bf7dc506e8743ba1ec5bd3325c91818b9192e40e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3.9 to 3.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 3.9 | 3 | 3 | [run](https://argusic.com/run/9078e19e-661b-46da-96d4-cf337dc571dd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 installed but project requires ^20.19.0 || ^22.12.0 || >=23`
- 1 min: `npm install without optionalDependencies leaves cloakbrowser missing; tsc fails on src/cloak.ts`
- 3 min: `No Google Chrome/chromium binary available on system; patchright install chrome needs root for apt deps`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
