# scholar-skill

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/EESJGong/scholar-skill, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/scholar-skill

## Pinned environment

- Project commit: `c7cfa2aa305dcf85b3b824019878610175662f9b`
- Test commit: `c7cfa2aa305dcf85b3b824019878610175662f9b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 1.8 to 1.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 1.5 | 1.8 | 3 | 3 | [run](https://argusic.com/run/68324081-b2f5-4306-afb3-13063dc5379b) |
| 2 | pass with mocks | 92 | 2 | 1.8 | 2 | 2 | [run](https://argusic.com/run/9fa5828f-a717-4e84-a074-f91b3382c32f) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pip install rejected by externally-managed-environment (PEP 668)`
- 0.3 min: `replace-placeholders.py EOFError with piped stdin`
- 0.2 min: `semi mode configure.py EOFError on interactive prompts`

Attempt 2:

- 1 min: `System Python 3.12 lacks PyYAML and pip is blocked by PEP 668 (ExternallyManagedEnvironment)`
- 1 min: `configure.py in manual mode with a nonexistent vault path prompts for 'Create this directory?' and crashes with EOFError on piped stdin`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
