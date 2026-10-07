# apinto

**Verdict: runs.** Argusic Score 82.9 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eolinker/apinto, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/apinto

## Pinned environment

- Project commit: `708a2ec565a0ae91d9206ca08a9858fe2729d1e3`
- Test commit: `708a2ec565a0ae91d9206ca08a9858fe2729d1e3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.2 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 82.86 | 14 | 14.2 | 7 | 1 | [run](https://argusic.com/run/8ce71ec5-a50a-474a-a6c0-6ea7b87d8e9d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.25.0+ compiler not found in container`
- `drivers/plugins/gzip/gzip_test.go: TestFilter/wantCompress SIGSEGV (nil pointer dereference)`
- `drivers/plugins/params-check/check_test.go: can not find body param '$.search[0].val'`
- `drivers/plugins/params-check-v2/check_test.go: build failed - MockHeaderReader missing SetCookie method`
- `drivers/service/send_test.go: ':invalid balance' - depends on external discovery service`
- `drivers/output/syslog/output_test.go: connection refused on tcp 127.0.0.1:514`
- `node/fasthttp-client/client_test.go: ProxyTimeout test fails connecting to 127.0.0.1:8099`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
