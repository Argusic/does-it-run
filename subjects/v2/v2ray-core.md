# v2ray-core

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/v2ray/v2ray-core, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/v2ray-core

## Pinned environment

- Project commit: `d80440f3d57b45c829dbf513306f7adf9a0f3f76`
- Test commit: `d80440f3d57b45c829dbf513306f7adf9a0f3f76`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 16.9 to 17.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 17.4 | 1 | 1 | [run](https://argusic.com/run/5aaef0f0-db49-4a3e-82d0-7ffb3bec9145) |
| 2 | pass | 100 | 3 | 16.9 | 3 | 3 | [run](https://argusic.com/run/46747944-f276-407f-85d5-cba75a6b8011) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `qtls-go1-15 v0.1.0 init() panics on Go >= 1.19 because crypto/tls struct layouts changed (ClientSessionState, ClientHelloInfo)`

Attempt 2:

- 5 min: `qtls-go1-15 init() panics on Go 1.22+ because tls.ClientSessionState struct changed between Go 1.15 and 1.22`
- 2 min: `crypto/hmac: hash generation function does not produce unique values in proxy/vmess/aead/kdf.go`
- 1 min: `Go 1.15 required but not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
