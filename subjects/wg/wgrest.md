# wgrest

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/suquant/wgrest, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/wgrest

## Pinned environment

- Project commit: `79d07f72b271a51b5f6cb2153354ec1695fe06ab`
- Test commit: `79d07f72b271a51b5f6cb2153354ec1695fe06ab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 2 | 2.8 | 2 | 1 | [run](https://argusic.com/run/5d5ca0dd-38f1-42e5-9226-2e69f336b85e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `no Go toolchain present and no root to install a system package`
- `WireGuard device create returns 'operation not permitted'; wg/wg-quick/ip absent and no CAP_NET_ADMIN/root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
