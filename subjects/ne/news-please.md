# news-please

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fhamborg/news-please, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/news-please

## Pinned environment

- Project commit: `f899850be2bb0059da101c13502ec88af057f974`
- Test commit: `f899850be2bb0059da101c13502ec88af057f974`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 4.9 to 11.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 5 | 11.8 | 0 | 0 | [run](https://argusic.com/run/898bea8d-6bd5-445c-8732-75798a5cc59d) |
| 2 | pass | 100 | 2 | 4.9 | 3 | 3 | [run](https://argusic.com/run/19bfa82f-6283-4262-97bb-00334ce68156) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Debian Python 3.12 blocks system-wide pip install due to externally-managed-environment`
- `newspaper4k prints warning that nltk is not installed, disabling optional NLP features`
- `Example scripts (downloadfromurl.py, downloadfromfile.py) contain hardcoded author machine paths`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
