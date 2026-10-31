# bluebox

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/VectorlyApp/bluebox, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/bluebox

## Pinned environment

- Project commit: `1021d39243f6e64d6441ff3891d0c868cea95fec`
- Test commit: `1021d39243f6e64d6441ff3891d0c868cea95fec`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 2.8 | 1 | 1 | [run](https://argusic.com/run/4e68f31b-999a-4847-9c53-60a8173c436d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `2 tests failed due to asyncio event loop handling: test_handle_unknown_message_returns_false in both AsyncWindowPropertyMonitorMessageHandling and AsyncInteractionMonitorMessageHandling`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
