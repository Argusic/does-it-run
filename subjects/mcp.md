# mcp

**Verdict: runs.** Argusic Score 97.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/awslabs/mcp, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/mcp

## Pinned environment

- Project commit: `e9f2439c08814ca478a143712d97eac3b27a25d6`
- Test commit: `e9f2439c08814ca478a143712d97eac3b27a25d6`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 12 to 42 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/913b0900-ea9c-4f85-9253-fd469cf270e1) |
| 2 | pass | 100 | 12 | 12 | 0 | 0 | [run](https://argusic.com/run/ad06f6f6-0c03-4d6d-ba5d-62c38e73569e) |
| 3 | pass | 94.29 | 8 | 35 | 7 | 5 | [run](https://argusic.com/run/0e5f4619-ec71-4aa1-ace3-f3bda50ec969) |

## What was observed on a clean machine

Attempt 3:

- 2 min: `uv package manager not installed in container`
- 1 min: `elasticache-mcp-server pyproject.toml missing pytest as dev dependency`
- 1 min: `openapi-mcp-server pyproject.toml missing pytest as dev dependency`
- 1 min: `roda-mcp-server pyproject.toml missing pytest as dev dependency`
- 1 min: `amazon-sns-sqs-mcp-server requires AWS config/credentials at startup`
- `aws-iot-sitewise-mcp-server signal handler prints to closed stdout after stdin closes`
- `Full test suites for cloudwatch-mcp-server, dynamodb-mcp-server, and aws-for-sap-management-mcp-server hang/timeout, likely waiting on live AWS services or Docker`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
