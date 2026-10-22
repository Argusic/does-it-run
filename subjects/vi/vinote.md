# ViNote

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zrt-ai-lab/ViNote, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/vinote

## Pinned environment

- Project commit: `e8e46a144caa718eb85bf053619892fc261fc1f9`
- Test commit: `e8e46a144caa718eb85bf053619892fc261fc1f9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15 to 15 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 15 | 3 | 3 | [run](https://argusic.com/run/10c9226a-2714-4628-a3ad-e91fd8f7bf5b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv not found in PATH`
- 1 min: `pytest module not found at import`
- 2 min: `test_content_generation.py and test_reasoning_effort_config.py fail on sibling imports`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
