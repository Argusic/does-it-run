# agent-toolkit-for-aws

**Verdict: runs.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aws/agent-toolkit-for-aws, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agent-toolkit-for-aws

## Pinned environment

- Project commit: `dda61487cb4fa8b6dbc75ad4e27c2181adc9d058`
- Test commit: `dda61487cb4fa8b6dbc75ad4e27c2181adc9d058`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 4 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 0.5 | 4 | 4 | 0 | [run](https://argusic.com/run/273a9e50-3438-4fbc-89f0-ccea6890f0ee) |
| 2 | pass with mocks | 84 | 12 | 8.3 | 5 | 3 | [run](https://argusic.com/run/f3748797-91f4-406c-a94d-feab784c1ac3) |

## What was observed on a clean machine

Attempt 1:

- `agents-pay portability test: httpx not found in isolated copy (2 checks failed)`
- `agents-pay x402 policy tests: 4 pre-existing failures (exit code mismatches)`
- `agents-pay node.js security test: missing dist/ (needs tsc build)`
- `markdownlint-cli2 requires Node >=22 but only Node 18 available; used older compatible version 0.18`

Attempt 2:

- 1 min: `plugins/aws-core/skills/aws-observability out of sync with canonical skills/core-skills/aws-observability`
- 1 min: `packages/openclaw expected staged skill scripts under skills/agents-pay/scripts/ but directory was empty (needed by test_setup_openclaw.py)`
- `Node markdown linter requires Node >=20 (have v18) for /v regex flags; gitleaks binary not found in container`
- `elasticache test_connection.py requires valkey/boto3 runtime; oracle test requires oracledb; marketplace test_event_publisher has no collected tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
