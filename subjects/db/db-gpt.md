# DB-GPT

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eosphoros-ai/DB-GPT, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/db-gpt

## Pinned environment

- Project commit: `ca9f014cb3ead157ca2ee6ce645658f5fb55138c`
- Test commit: `ca9f014cb3ead157ca2ee6ce645658f5fb55138c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.6 to 16.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 16.6 | 4 | 4 | [run](https://argusic.com/run/a2a123bc-d71b-49ed-bf2f-a66cd4bc76c8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Optional litellm dependency missing for proxy model tests (ModuleNotFoundError)`
- 1 min: `pilot_template directory not accessible from workspace_provisioning module in development mode (6 workspace tests failed)`
- 2 min: `skill_upload endpoint had no path traversal validation (3 tests failed)`
- 3 min: `attachment_react_adapter tests patched agentic_data_api.StreamingResponse but endpoint now uses _AgentStreamingResponse (2 tests failed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
