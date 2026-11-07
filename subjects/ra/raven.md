# Raven

**Verdict: runs with mocks.** Argusic Score 88.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/EverMind-AI/Raven, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/raven

## Pinned environment

- Project commit: `e84152c52fe4a5a1b87f2e605f4d85afee2ff452`
- Test commit: `e84152c52fe4a5a1b87f2e605f4d85afee2ff452`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 10.2 to 35 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14 | 10.2 | 0 | 0 | [run](https://argusic.com/run/22e6329d-c907-44d5-8557-27522b3081bd) |
| 2 | pass with mocks | 85.33 | 0.5 | 35 | 3 | 2 | [run](https://argusic.com/run/7b808596-995b-4da6-9acd-9d962b4d2966) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `test_an_empty_message_file_is_a_usage_error: Rich word-wraps error output, breaking exact 'is empty' string match`
- 5 min: `test_bold_accent_renders_styled_not_bare: Rich 14.x consolidates nested theme colors into parent [bold] segments, dropping separate ANSI color escape`
- 1 min: `test_resolve_node_dir_answers_each_case_it_exists_for: install.sh test expects node-v22.20.0-x provisioning path but gets sysbin directly`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
