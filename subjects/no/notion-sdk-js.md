# notion-sdk-js

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/makenotion/notion-sdk-js, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/notion-sdk-js

## Pinned environment

- Project commit: `51268112018fe42286c8597484989c8e37028376`
- Test commit: `51268112018fe42286c8597484989c8e37028376`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 10.1 to 30.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 10.1 | 0 | 0 | [run](https://argusic.com/run/f17bd75d-3201-4ce0-a6e8-4b3bcc19cbfa) |
| 2 | pass with mocks | 92 | 16 | 30.5 | 1 | 1 | [run](https://argusic.com/run/ff94eddd-ba8a-485f-9ad2-21b51536ffc6) |

## What was observed on a clean machine

Attempt 2:

- `Compatibility test (compatibility.test.ts) hangs due to TypeScript compiler API resource constraints in the container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
