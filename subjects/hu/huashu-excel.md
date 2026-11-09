# huashu-excel

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alchaincyf/huashu-excel, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/huashu-excel

## Pinned environment

- Project commit: `2492fabbafc8498496edd70f7e2354016a8dd06e`
- Test commit: `2492fabbafc8498496edd70f7e2354016a8dd06e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.4 to 9.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 9.4 | 3 | 3 | [run](https://argusic.com/run/cce4563c-1481-459f-bccc-d47748de87be) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Python is PEP 668 externally managed; pip install pandas/openpyxl refused`
- 30 min: `make_report.py xlsx output failed its own verify_xlsx.py gate: 18pt title clipped by 16pt row height, freeze_panes A2 froze a blank row, body text sat on the wrap edge`
- 4 min: `verify_visual.py exits 2 without playwright`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
