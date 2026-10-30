# Misaka-Agent

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Luciole-Studio/Misaka-Agent, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/misaka-agent

## Pinned environment

- Project commit: `3bcf7a33fb33109d03e368873570d0a7b402b210`
- Test commit: `3bcf7a33fb33109d03e368873570d0a7b402b210`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.1 to 22.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 1 | 22.1 | 3 | 2 | [run](https://argusic.com/run/754ad23c-60fe-483b-8d46-c83e70f9f8d4) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `test_research_missing_session.py expected 'No model is available' but current code raises 'The Sister roster is empty; research tasks cannot be assigned.' first on resume with no Sisters/roster`
- 10 min: `test_pdf_ocr_routing.py::test_a_reread_put_off_and_then_answered_forgets_the_misses fails because it needs the optional ocrmypdf system package on PATH`
- 10 min: `fd and pdftotext system packages absent (no root); project bundles them in its prebuilt release archive`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
