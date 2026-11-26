# Stealth-Requests

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jpjacobpadilla/Stealth-Requests, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/stealth-requests

## Pinned environment

- Project commit: `55886f4f49e9922e82d24d68472293ed449f9281`
- Test commit: `55886f4f49e9922e82d24d68472293ed449f9281`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.1 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.2 | 1.1 | 0 | 0 | [run](https://argusic.com/run/2f0e6b9f-766b-4793-b644-9c5205b7f826) |
| 2 | pass | 100 | 1 | 2.2 | 1 | 1 | [run](https://argusic.com/run/e5d3abf3-f443-4dce-aac5-2d708a850608) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `test_unresolvable_version_leaves_curl_cffi_headers_intact failed: curl_cffi 0.17.0 default UA is Windows, not macOS`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
