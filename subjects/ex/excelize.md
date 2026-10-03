# excelize

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/qax-os/excelize, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/excelize

## Pinned environment

- Project commit: `2badfcd5841d0d88b0ffea119f5a2f3c53b4910b`
- Test commit: `2badfcd5841d0d88b0ffea119f5a2f3c53b4910b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 10.7 to 53.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 53.4 | 2 | 2 | [run](https://argusic.com/run/edfbff9e-a148-4faa-bfc9-5a64e9600aeb) |
| 2 | pass | 100 | 15 | 10.7 | 2 | 2 | [run](https://argusic.com/run/e15b83cc-87dc-437e-9618-91505ad7605d) |
| 3 | pass | 100 | 2.5 | 16.2 | 1 | 1 | [run](https://argusic.com/run/72a5f1b2-c1c5-49de-a6b1-91be45196ac4) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.25.0+ not installed in container`
- 1 min: `TestZip64 times out - generates 131x1000 cells of max-size content exceeding 10m default test timeout`

Attempt 2:

- 2 min: `Go 1.25.0 was not pre-installed in the container environment`
- 5 min: `Full test suite killed (signal: killed) after 317s due to OOM/timeout on TestZip64`

Attempt 3:

- 5 min: `go test ./... (full suite) killed by OOM in 770MB container when running all 442 tests together`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
