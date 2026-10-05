# beyla

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/grafana/beyla, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/beyla

## Pinned environment

- Project commit: `d6e1d67280eaa95c840db8ca1b31964ddc450ebc`
- Test commit: `d6e1d67280eaa95c840db8ca1b31964ddc450ebc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 43.7 to 52.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 52.5 | 0 | 0 | [run](https://argusic.com/run/6e02efbf-261e-4d2b-b19e-8eadd2cc54e0) |
| 2 | fail | 20 | 42 | 43.7 | 5 | 5 | [run](https://argusic.com/run/1c2ab596-ecaa-42c1-8b48-51be136da71f) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go not pre-installed in container`
- 10 min: `Git submodule .obi-src empty at checkout`
- 13 min: `BPF .o bytecode files missing from vendor directory (go:embed targets)`
- 10 min: `Source build fails with 21+ undefined BPF-generated type errors`
- 7 min: `Disk full during LLVM extraction (7.8G total, 3.2G trash remaining)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
