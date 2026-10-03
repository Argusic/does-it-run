# cloudflared

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cloudflare/cloudflared, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/cloudflared

## Pinned environment

- Project commit: `f9676c585623c86c0a48dbb6ae80840b4c834718`
- Test commit: `f9676c585623c86c0a48dbb6ae80840b4c834718`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 44 to 44 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 43 | 44 | 5 | 5 | [run](https://argusic.com/run/758cfd6d-8673-44a9-850e-353d950417c1) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go 1.27+ not found in PATH`
- 5 min: `TestSupportedCurvesNegotiation fails on Go 1.27: P256Kyber768Draft00 no longer advertised in TLS handshakes`
- `ICMP/ping tests fail: GID 1001 outside ping_group_range`
- `quic TestDatagram times out at 30s when run with resource-heavy packages (sshgen, token)`
- 3 min: `golangci-lint v1.62 built with Go 1.23 cannot parse Go 1.26 config`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
