# patchright-python

**Verdict: runs.** Argusic Score 98 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Kaliiiiiiiiii-Vinyzu/patchright-python, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/patchright-python

## Pinned environment

- Project commit: `c4064f5833c811d99772aabefee8984c51322ace`
- Test commit: `c4064f5833c811d99772aabefee8984c51322ace`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.6 to 37.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 37.1 | 0 | 0 | [run](https://argusic.com/run/73b82d6d-041b-40fb-b53b-5577d6caf7c5) |
| 2 | pass | 96 | 10 | 9.6 | 5 | 4 | [run](https://argusic.com/run/16fa0014-a4d9-44cc-9a9e-d8a8aa57278b) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `System Python is externally managed (PEP 668)`
- 1 min: `pixelmatch 0.4.0 dropped from_PIL_to_raw_data`
- 2 min: `Missing test dependencies: autobahn, twisted, pyopenssl, service-identity, asyncio-atexit`
- `6 sync test failures: SSL cert infrastructure (sign_count, security_details, ssl timing), signal handler in subprocess, page_pause timeout (Xvfb quirk)`
- 0.5 min: `async test failure: asyncio-atexit not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
