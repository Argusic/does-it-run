# claude-canvas

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AgriciDaniel/claude-canvas, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/claude-canvas

## Pinned environment

- Project commit: `05b808cafd906bb3b8ff1c597ed8cd33ff5145c0`
- Test commit: `05b808cafd906bb3b8ff1c597ed8cd33ff5145c0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.6 to 1.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 1.6 | 1 | 1 | [run](https://argusic.com/run/989b7f92-8fc6-474a-8bcd-df4567654402) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `canvas_template.py references SCRIPT_DIR but never defines it, causing NameError on templates with post_layout (flowchart, knowledge-graph, mind-map)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
