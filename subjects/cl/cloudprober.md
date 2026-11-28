# cloudprober

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cloudprober/cloudprober, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/cloudprober

## Pinned environment

- Project commit: `a36f8d2d4b0d6251d0f45f1c7ae8787d43b3a487`
- Test commit: `a36f8d2d4b0d6251d0f45f1c7ae8787d43b3a487`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.6 to 16.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 16.6 | 4 | 4 | [run](https://argusic.com/run/25fb3473-8220-4cd9-85ca-595f42965271) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `[email test] TestNewEmailNotifier/default_localhost failed because hostname was 'ace3fa80ada7' rather than 'localhost'`
- `[probes/http] IPv6 tests fail: 'bind: cannot assign requested address' on [::1]`
- `[probes/ping] DGRAM_6 test fails: 'sendto: cannot assign requested address' on IPv6 addresses`
- `[probes/udp] All UDP probe tests fail: resolves localhost to [::1] which doesn't work without IPv6`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
