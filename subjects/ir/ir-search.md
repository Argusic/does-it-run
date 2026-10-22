# ir-search

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/djfksjd/ir-search, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ir-search

## Pinned environment

- Project commit: `9ef913a40f3a06bbd08715078b947c60c0666fe0`
- Test commit: `9ef913a40f3a06bbd08715078b947c60c0666fe0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.8 to 3.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 3.8 | 1 | 1 | [run](https://argusic.com/run/4e59104f-27ea-4d94-8d1f-408616067b49) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip3 install 'curl_cffi>=0.15' failed with 'externally-managed-environment' (PEP 668) on the container's system Python; install.sh hit the same non-fatal error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
