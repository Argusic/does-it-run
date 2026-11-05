# watermill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ThreeDotsLabs/watermill, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/watermill

## Pinned environment

- Project commit: `080d4b4e7fe6105ab880d1becd5cf91af0235d8c`
- Test commit: `080d4b4e7fe6105ab880d1becd5cf91af0235d8c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.3 to 20.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3.3 | 0 | 0 | [run](https://argusic.com/run/9f6eb7f2-869c-4e52-9a14-5247af0dac11) |
| 2 | pass | 100 | 27 | 20.6 | 3 | 3 | [run](https://argusic.com/run/a5477a57-31fc-45e3-8047-9eb964b2fe9e) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `No Go toolchain in container (go: not found)`
- 12 min: `No Docker/Java in container, so example's docker-compose path (kafka:9092, redpanda/golang images) could not be used`
- 8 min: `go test ./... initial run needed module downloads, and the mill tool separate module (tools/mill) fails to build: undefined: http2.TrailerPrefix (grpc v1.81.0 with golang.org/x/net v0.54.0)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
