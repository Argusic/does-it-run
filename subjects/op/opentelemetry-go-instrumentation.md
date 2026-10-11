# opentelemetry-go-instrumentation

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/open-telemetry/opentelemetry-go-instrumentation, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/opentelemetry-go-instrumentation

## Pinned environment

- Project commit: `24123c2a5d46db206770d28434b07b1d63943b09`
- Test commit: `24123c2a5d46db206770d28434b07b1d63943b09`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.4 to 7.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.2 | 7.4 | 4 | 4 | [run](https://argusic.com/run/4fa3546d-0a9f-4c4c-9eee-c55f54bc773f) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `Go not installed in container`
- 0.3 min: `clang/llvm-strip not installed (needed to compile eBPF .o files for tests)`
- 0.2 min: `BPF .o files missing , go generate failed: stdbool.h not found via clang built-in include path`
- `TestEBPFNewSamplingConfigDefault fails: operation not permitted for set memlock rlimit`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
