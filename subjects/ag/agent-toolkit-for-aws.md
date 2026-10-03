# agent-toolkit-for-aws

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aws/agent-toolkit-for-aws, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agent-toolkit-for-aws

## Pinned environment

- Project commit: `dda61487cb4fa8b6dbc75ad4e27c2181adc9d058`
- Test commit: `dda61487cb4fa8b6dbc75ad4e27c2181adc9d058`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4 to 4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 0.5 | 4 | 4 | 0 | [run](https://argusic.com/run/273a9e50-3438-4fbc-89f0-ccea6890f0ee) |

## What was observed on a clean machine

Attempt 1:

- `agents-pay portability test: httpx not found in isolated copy (2 checks failed)`
- `agents-pay x402 policy tests: 4 pre-existing failures (exit code mismatches)`
- `agents-pay node.js security test: missing dist/ (needs tsc build)`
- `markdownlint-cli2 requires Node >=22 but only Node 18 available; used older compatible version 0.18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
