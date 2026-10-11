# awesome-vibecoded-saas

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Anil-matcha/awesome-vibecoded-saas, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/awesome-vibecoded-saas

## Pinned environment

- Project commit: `a619af1f0ca938ef78b9fbf7558a45f6c5b31aea`
- Test commit: `a619af1f0ca938ef78b9fbf7558a45f6c5b31aea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.2 to 1.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 1.2 | 2 | 2 | [run](https://argusic.com/run/510b5e84-23a2-433a-941d-7a2ab8883e75) |

## What was observed on a clean machine

Attempt 1:

- `python3 -c import jsonschema failed: ModuleNotFoundError (probe only; repo validator is stdlib-only per scripts/validate.py docstring and README)`
- `network probe to json-schema.org returned HTTP 403 (probe only; not needed by the repo)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
