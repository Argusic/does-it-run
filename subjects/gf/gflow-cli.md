# gflow-cli

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ffroliva/gflow-cli, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/gflow-cli

## Pinned environment

- Project commit: `a5d0e39853b07eed3612c75cee8bc3f0056a6c55`
- Test commit: `a5d0e39853b07eed3612c75cee8bc3f0056a6c55`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 22.2 to 27.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 27.3 | 0 | 0 | [run](https://argusic.com/run/a9e49985-13cf-4c06-954f-2f2793aa81d5) |
| 2 | pass | 100 | 2.5 | 22.2 | 1 | 1 | [run](https://argusic.com/run/d067afca-521c-4bb4-a830-e0db5bbbe7e2) |

## What was observed on a clean machine

Attempt 2:

- 15 min: `test_verification_error_on_browser_cookie_decryption_error failed because is_playwright_chrome_channel_available was not patched in the test; the container lacks system Google Chrome, so channel_for_profile returns None instead of "chrome",`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
