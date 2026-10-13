# super

**Verdict: runs with mocks.** Argusic Score 52.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spr-networks/super, licensed BSD-3-Clause, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/super

## Pinned environment

- Project commit: `0010d454a60a428dd779f3fcece8cd6db8254a9b`
- Test commit: `0010d454a60a428dd779f3fcece8cd6db8254a9b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 11.7 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 12.4 | 0 | 0 | [run](https://argusic.com/run/e96bb7c5-d2b8-4d36-b80f-4c075f1dbe8d) |
| 2 | pass with mocks | 85.33 | 12 | 11.7 | 3 | 2 | [run](https://argusic.com/run/2c663cba-8f8e-4770-bd64-638375fd733f) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Go binary not found in container; installed go1.26.6 manually from golang.org`
- 2 min: `Missing /test/configs and state directories for API test environment`
- `31 nftables/netlink tests fail with 'operation not permitted' and 1 fails with 'nft: not found' and 1 with 'ip: not found' , all require root/net_admin privileges`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
