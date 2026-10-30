# Office2PDF

**Verdict: runs with mocks.** Argusic Score 46 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/evgo2017/Office2PDF, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/office2pdf

## Pinned environment

- Project commit: `b3a9b8dc00cc01905c95307ec621ac19b4795f0e`
- Test commit: `b3a9b8dc00cc01905c95307ec621ac19b4795f0e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 4.3 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 3 | 4.3 | 3 | 0 | [run](https://argusic.com/run/7459d6c6-9fbe-476d-ae64-cb46c7fb2fe1) |
| 2 | pass with mocks | 92 | 15 | 18.7 | 3 | 3 | [run](https://argusic.com/run/7b27c87f-caf8-4978-bae1-fea3f82d8b7b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `The tkinter GUI module is unavailable: python3-tk is not installed and cannot be pip-installed ('no matching distribution for python3-tk'); installing it requires root, which does not exist here.`
- 1 min: `pywin32 (win32com) has no Linux distribution; pip returned 'No matching distribution found for pywin32' on both the system Python and a fresh venv. pywin32 and the COM calls it enables are Windows-only.`
- 1 min: `Office2PDF is a Windows-only desktop app (tkinter GUI driving MS Word/Excel/PowerPoint via COM). The container is Ubuntu 24.04 Linux with no Wine, no LibreOffice, and no root, so the program cannot launch here regardless of dependencies.`

Attempt 2:

- 10 min: `win32com.client and pythoncom not available on Linux (Windows-only COM libraries)`
- 3 min: `tkinter not installed (missing python3-tk package)`
- 1 min: `fpdf2 cannot encode CJK characters with default Helvetica font`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
