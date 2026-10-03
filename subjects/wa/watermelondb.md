# WatermelonDB

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Nozbe/WatermelonDB, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/watermelondb

## Pinned environment

- Project commit: `5c463222ecd79928861385bac94b486fcc7623d4`
- Test commit: `5c463222ecd79928861385bac94b486fcc7623d4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.2 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.7 | 4.2 | 2 | 2 | [run](https://argusic.com/run/d41bb8c1-b234-4958-bc61-aa76b2062e49) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm install failed due to peer dependency conflicts with @testing-library/react-hooks requiring react ^16.9.0 || ^17.0.0 but react@18.3.1 installed`
- 1.5 min: `All 80 test suites failed with TypeError: Cannot read properties of undefined (reading AsymmetricMatcher) in jest-diff`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
