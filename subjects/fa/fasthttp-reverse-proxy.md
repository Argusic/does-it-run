# fasthttp-reverse-proxy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yeqown/fasthttp-reverse-proxy, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/fasthttp-reverse-proxy

## Pinned environment

- Project commit: `3b0dcb225a9ffecd8b3e70436d0c0f78671c104c`
- Test commit: `3b0dcb225a9ffecd8b3e70436d0c0f78671c104c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.5 to 15.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 15.5 | 4 | 4 | [run](https://argusic.com/run/8f4d1793-15c6-440d-8454-b5762809a945) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `no Go toolchain in the container`
- 6 min: `go build ./.../go test ./... failed: examples/https-reverse-proxy had two func main in one package (tlscert.go + proxy.go)`
- 1 min: `go vet flagged benchmark/ws_proxy_benchmark.go:44: misuse of unbuffered os.Signal channel`
- 4 min: `the plain HTTP example hardcoded localhost:8080, which in this container resolved to the stale TLS backend, so the demo proxy returned 500`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
