# openclacky

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/clacky-ai/openclacky, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/openclacky

## Pinned environment

- Project commit: `261aabd59d76e32fa8b8baa3aa7a4147b150236e`
- Test commit: `261aabd59d76e32fa8b8baa3aa7a4147b150236e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 3.8 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 1.5 | 3.8 | 2 | 2 | [run](https://argusic.com/run/fa32c943-ca21-4c5f-9975-11d0094ff79b) |
| 2 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/8d253445-4753-4bd8-a788-54d16664f77c) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Ruby not installed , had to install via mise`
- `2 test failures: IPv6 loopback unavailable (container), scripts path check (running from repo source)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
