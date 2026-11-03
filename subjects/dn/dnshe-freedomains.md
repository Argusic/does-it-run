# DNSHE-FreeDomains

**Verdict: runs with mocks.** Argusic Score 89.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dnshe/DNSHE-FreeDomains, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dnshe-freedomains

## Pinned environment

- Project commit: `bbe16aa0119d952ef7add9b074a297e87374d23a`
- Test commit: `bbe16aa0119d952ef7add9b074a297e87374d23a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 1.9 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 4.6 | 0 | 0 | [run](https://argusic.com/run/c461a8e3-e9ed-4805-9788-c38738f59afd) |
| 2 | pass with mocks | 87 | 5 | 1.9 | 4 | 3 | [run](https://argusic.com/run/2562417c-5b87-4374-b7d4-5721763b3b6c) |

## What was observed on a clean machine

Attempt 2:

- `Bash-only pipefail flag rejected by /bin/sh before project commands ran`
- 1 min: `Temporary HTTPS mock exited when its launcher shell ended, causing connection refused`
- 1 min: `Mock matched per_page=100 as its per_page=1 rate-limit case`
- `PHP runtime is unavailable, so the PHP example could not be executed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
