# agent-safe-pipeline

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/decionis/agent-safe-pipeline, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/agent-safe-pipeline

## Pinned environment

- Project commit: `2126d70fb4cecfcadf8adb3e80fa98ab2892c911`
- Test commit: `2126d70fb4cecfcadf8adb3e80fa98ab2892c911`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.9 to 15.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 15.9 | 3 | 3 | [run](https://argusic.com/run/ef6fd517-1ba8-40eb-a0c9-059427799acb) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `System node is v18.19.1 but the repo requires Node >=22.14.0 (and pnpm/corepack were absent)`
- 3 min: `The Go toolchain needed by the govern contract test (go build ./cmd/govern) was missing`
- `The recursive workspace test run initially failed at @decionis/govern-contract with ERR_TEST_FAILURE/ERR_ASSERTION because the Go binary could not be built`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
