# abstruse

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bleenco/abstruse, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/abstruse

## Pinned environment

- Project commit: `39de5c2b0e8d93d8b402d8df504fc327a37ec4ba`
- Test commit: `39de5c2b0e8d93d8b402d8df504fc327a37ec4ba`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 9.6 to 76.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 76.5 | 0 | 0 | [run](https://argusic.com/run/f83d9642-1ce4-4234-8413-8afe93525095) |
| 2 | pass | 100 | 10 | 9.6 | 3 | 3 | [run](https://argusic.com/run/c96f7d92-4b69-4789-9ca9-93eb117f08c9) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go not installed in container`
- 4 min: `Build tools (protoc, protoc-gen-go, protoc-gen-go-grpc, statik, wire, reflex) not installed`
- 1 min: `protoc failed due to missing well-known types include path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
