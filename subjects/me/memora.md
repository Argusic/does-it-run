# memora

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agentic-box/memora, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/memora

## Pinned environment

- Project commit: `c5624e8303f0670c0f1fd03ae7900786ab7c95a3`
- Test commit: `c5624e8303f0670c0f1fd03ae7900786ab7c95a3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.3 to 44.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 9.3 | 0 | 0 | [run](https://argusic.com/run/c2b86b00-f1dd-44c4-b156-d077ed1cbd5b) |
| 2 | pass | 100 | 0.17 | 44.9 | 2 | 2 | [run](https://argusic.com/run/e24cd0a3-410a-4de8-89bb-e2b4d9ebdcc4) |

## What was observed on a clean machine

Attempt 2:

- `Datetime deprecation warnings: storage.py uses deprecated datetime.utcnow() in 5+ locations`
- `Externally-managed environment blocked system pip (PEP 668)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
