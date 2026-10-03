# opensre

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Tracer-Cloud/opensre, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/opensre

## Pinned environment

- Project commit: `c0ff91eb0ef14c35093f541a3a6e787f6a9e2f03`
- Test commit: `c0ff91eb0ef14c35093f541a3a6e787f6a9e2f03`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 44.1 to 44.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 43 | 44.1 | 1 | 1 | [run](https://argusic.com/run/e30854dd-c8de-41d1-a66e-2b21d9ba8eb5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `test_composite_fingerprint_hashes_stable_local_and_ci_signals failed because container runtime detection added 'container' to fingerprint components in Docker environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
