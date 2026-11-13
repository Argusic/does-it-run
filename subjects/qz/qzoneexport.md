# QZoneExport

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ShunCai/QZoneExport, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/qzoneexport

## Pinned environment

- Project commit: `7e0218fab29316ca28b99a7c63deb0627002d271`
- Test commit: `7e0218fab29316ca28b99a7c63deb0627002d271`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 3.5 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 8.8 | 2 | 2 | [run](https://argusic.com/run/cc7f3c25-2d54-4d1f-a014-65f8905dc72d) |
| 2 | pass with mocks | 92 | 5.6 | 3.5 | 2 | 2 | [run](https://argusic.com/run/561492e6-dc11-4a30-b46b-3662317de54e) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `System Node.js v18.19.1 does not meet project requirement of Node.js >=22. npm install failed with syntax errors in wxt (node:util parseEnv).`
- 0.5 min: `2 of 506 tests failed due to timezone mismatch: tests expected China Standard Time (UTC+8) but container runs UTC.`

Attempt 2:

- 2.5 min: `System Node.js (v18.19.1) too old; requires Node >=22`
- 0.5 min: `2 tests failed due to timezone mismatch (tests assume Asia/Shanghai but container runs UTC)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
