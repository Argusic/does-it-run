# urllib3

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/urllib3/urllib3, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/urllib3

## Pinned environment

- Project commit: `ed0ed075c6b93f7c515ebd3abe9a7248507ef8c5`
- Test commit: `ed0ed075c6b93f7c515ebd3abe9a7248507ef8c5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.8 to 14.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 14.8 | 4 | 4 | [run](https://argusic.com/run/93fefd2b-e7c9-4e68-a71d-556a6176869f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `IPv6 not available on loopback (errno 99) caused hypercorn socket binding to fail`
- 2 min: `test_client_intermediate failed because stock hypercorn doesn't expose client_cert_name in TLS extensions`
- 1 min: `ipv6_san_proxy_with_server fixture tried binding ::1 without checking HAS_IPV6`
- 1 min: `test_socks_with_invalid_username didn't use _set_up_fake_getaddrinfo, causing PySocks to fail on IPv6 resolution`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
