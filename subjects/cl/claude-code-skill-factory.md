# claude-code-skill-factory

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alirezarezvani/claude-code-skill-factory, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/claude-code-skill-factory

## Pinned environment

- Project commit: `ba18b31703542d9d7eda5f9ba94f0df65a59dddf`
- Test commit: `ba18b31703542d9d7eda5f9ba94f0df65a59dddf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 8.5 to 23.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 23 | 23.3 | 1 | 1 | [run](https://argusic.com/run/9e1709c1-e540-4b3a-944b-b0ac77dd6e01) |
| 2 | pass with mocks | 92 | 0 | 8.5 | 2 | 2 | [run](https://argusic.com/run/048641e1-97c3-4364-a8d2-e945d7db56e0) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `scrum-master-agent/prioritize_backlog.py had unused import from calculate_metrics causing import collision with social-media-analyzer`
- 2 min: `agent-factory/agent_generator.py missing blank line after YAML frontmatter causing output mismatch with expected_output.json`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
