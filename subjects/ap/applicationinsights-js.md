# ApplicationInsights-JS

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/ApplicationInsights-JS, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/applicationinsights-js

## Pinned environment

- Project commit: `10aa1209697fcdd081b81647799360bef3323a80`
- Test commit: `10aa1209697fcdd081b81647799360bef3323a80`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 58.3 to 58.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 52 | 58.3 | 3 | 3 | [run](https://argusic.com/run/1cbb04b2-080e-4857-a1d5-05ca5f4cc2e1) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `tools/pureAnnotations.mjs: ESM import { parse } from "acorn" fails in Rush+pnpm+Node 18 setup because acorn's exports array is not resolved correctly`
- 5 min: `Puppeteer test failure: Could not find Chrome (headless browser not installed)`
- 5 min: `TypeScript compilation error: Cannot find module @nevware21/ts-async in analytics-js tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
