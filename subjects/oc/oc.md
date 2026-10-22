# oc

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/only-cli/oc, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/oc

## Pinned environment

- Project commit: `8de20cfc5646d55ae7b29da802a47eea99a753f8`
- Test commit: `8de20cfc5646d55ae7b29da802a47eea99a753f8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.7 to 2.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.7 | 1 | 1 | [run](https://argusic.com/run/9615b3cf-98d0-4289-a56d-3b1dd8f513ab) |

## What was observed on a clean machine

Attempt 1:

- `IPv6 EADDRNOTAVAIL in fetch.test.js:524 , container lacks IPv6 loopback (::1)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
