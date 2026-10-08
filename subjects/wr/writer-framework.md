# writer-framework

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/writer/writer-framework, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/writer-framework

## Pinned environment

- Project commit: `53eef36becc2fbb35e83c2f20be46cb6ebb7484d`
- Test commit: `53eef36becc2fbb35e83c2f20be46cb6ebb7484d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.6 to 10.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 10.6 | 3 | 3 | [run](https://argusic.com/run/0b8fe6e2-7cd7-495e-bf25-2006786e1788) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `ModuleNotFoundError: No module named 'writer.ui' , ui.py was missing (needs frontend codegen)`
- 0.5 min: `pytest not found initially , build group dependencies not installed`
- 1.5 min: `npm build OOM on first attempt due to Node.js 18 vs required 22`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
