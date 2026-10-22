# Tracely-ai

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jwuthri-cloud/Tracely-ai, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/f31114c4-ee34-444b-a379-735121644cbe

## Pinned environment

- Project commit: `e6a37cddb0a62b4a4b925b0f517532e541daa208`
- Test commit: `e6a37cddb0a62b4a4b925b0f517532e541daa208`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.5 to 9.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 9.5 | 3 | 3 | [run](https://argusic.com/run/f31114c4-ee34-444b-a379-735121644cbe) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `uv command not found in PATH`
- 1 min: `pip install failed due to PEP 668 (externally-managed-environment)`
- `Node.js 18.19.1 too old for Next.js 16 (requires >=20.9.0) , frontend build fails`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
