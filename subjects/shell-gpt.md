# shell_gpt

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TheR1D/shell_gpt, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/shell-gpt

## Pinned environment

- Project commit: `a082bd5327ce0c4ef5a0284d9060e833be9444a6`
- Test commit: `a082bd5327ce0c4ef5a0284d9060e833be9444a6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.5 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 8.5 | 1 | 1 | [run](https://argusic.com/run/7d05128a-ebe5-4ccb-a64e-676cbd2821e5) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Config module fails at module load when no config file or API key exists: 'getpass()' prompts for API key on import, and 'Config.get()' uses 'if not value:' which treats float 0.0 (DEFAULT_TEMPERATURE) as falsy, raising 'Missing config key'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
