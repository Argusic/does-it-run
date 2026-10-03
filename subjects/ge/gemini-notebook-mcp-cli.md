# gemini-notebook-mcp-cli

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jacob-bd/gemini-notebook-mcp-cli, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/gemini-notebook-mcp-cli

## Pinned environment

- Project commit: `a7ace144d70f9a150e0951198d7014519cc6e970`
- Test commit: `a7ace144d70f9a150e0951198d7014519cc6e970`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8 to 8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 8 | 2 | 2 | [run](https://argusic.com/run/beb42fc7-0526-485e-905b-1463dc9f559f) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `test_login_force_bypasses_saved_profile_validation failed exit 1: select_auth_backend() returned None in container without Chrome`
- 2 min: `test_login_clear_bypasses_valid_saved_profile failed exit 1: same root cause`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
