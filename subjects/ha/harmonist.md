# harmonist

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GammaLabTechnologies/harmonist, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/harmonist

## Pinned environment

- Project commit: `6fd5941cce8c3f6f411fd14cde0daa663ccffa8f`
- Test commit: `6fd5941cce8c3f6f411fd14cde0daa663ccffa8f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.7 to 9.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 5.7 | 1 | 1 | [run](https://argusic.com/run/ce390074-7500-4bed-b489-97d57f21846c) |
| 2 | pass | 100 | 35 | 9.4 | 3 | 3 | [run](https://argusic.com/run/106f8e35-8c4b-4c62-a78b-7e6a7fc94420) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `lsof not installed: test_telemetry_webhook.sh could not run its live-POST/retry scenarios (4 of 7 scenarios skipped)`

Attempt 2:

- 2 min: `MANIFEST.sha256 stale after integration created AGENTS.md`
- 5 min: `Integration verifier found 3 errors: AGENTS.md had template placeholders, default Invariants, and CUSTOMIZE comments`
- `telemetry_webhook.sh test fails because lsof is missing from container (exit 127)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
