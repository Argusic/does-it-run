# newspaper

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/codelucas/newspaper, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/newspaper

## Pinned environment

- Project commit: `f8e3cb63c87ff53080fab77f4bafef2ecf8179f7`
- Test commit: `f8e3cb63c87ff53080fab77f4bafef2ecf8179f7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.4 to 4.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 4.4 | 3 | 3 | [run](https://argusic.com/run/991ba54c-f9ff-42e2-99e9-6b322bdf96ba) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `lxml.html.clean module split into separate lxml_html_clean package`
- 0.2 min: `NLTK punkt_tab resource missing (NLTK 3.10+ renamed punkt to punkt_tab)`
- 0.3 min: `Chinese expected text file (tests/data/text/chinese.txt) contained overlong-encoded C2 93 / C2 94 bytes instead of proper UTF-8 curly quotes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
