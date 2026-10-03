# gateway

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/envoyproxy/gateway, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/run/f760fda5-ff59-455f-a2b5-7499032ee92c

## Pinned environment

- Project commit: `1f9a811a5737f63e60925e023c8d634f0b9cf0e6`
- Test commit: `1f9a811a5737f63e60925e023c8d634f0b9cf0e6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 22.2 to 22.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 19 | 22.2 | 3 | 3 | [run](https://argusic.com/run/f760fda5-ff59-455f-a2b5-7499032ee92c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.27.1 not present in container environment`
- 1 min: `xds/translator testdata mismatch on merge-backends-consistent-hash test`
- `internal/wasm test suite hangs indefinitely due to TLS handshake to local test server`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
