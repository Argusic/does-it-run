# ttl

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lance0/ttl, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/ttl

## Pinned environment

- Project commit: `74cefd8839428ea9faf809894f143a537f06bf62`
- Test commit: `74cefd8839428ea9faf809894f143a537f06bf62`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.4 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2.1 | 12.4 | 3 | 3 | [run](https://argusic.com/run/e79b8f38-761c-4a91-9f4d-1ff9d565e2ad) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `Rust toolchain not pre-installed in container`
- 1 min: `setcap binary not available on PATH for granting cap_net_raw to binary`
- 1 min: `Raw ICMP sockets require CAP_NET_RAW or root, unavailable in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
