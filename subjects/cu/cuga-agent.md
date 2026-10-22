# cuga-agent

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cuga-project/cuga-agent, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/cuga-agent

## Pinned environment

- Project commit: `bd31b638b1d80983f400b3bf58afcced53d44457`
- Test commit: `bd31b638b1d80983f400b3bf58afcced53d44457`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 29.1 to 29.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.5 | 29.1 | 3 | 3 | [run](https://argusic.com/run/edad62f3-1928-4c73-a519-6fcf0e39cede) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `test_e2e_server_stack.py: subprocess.Popen(['python', ...]) fails because 'python' is not on PATH in this container`
- 0.3 min: `evolve extra was missing (altk_evolve module not found), causing 7 evolve retention tests and 1 evolve bundled hooks test to fail`
- 0.2 min: `test_agent_policy_isolation.py requires OPENAI_API_KEY env var; fails with credential error when absent`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
