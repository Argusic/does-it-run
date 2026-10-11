# kindling

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/harmonycloud/kindling, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/kindling

## Pinned environment

- Project commit: `034a8ce086e3f1a34be7c1b10cf4a163b8825541`
- Test commit: `034a8ce086e3f1a34be7c1b10cf4a163b8825541`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 66.2 to 66.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 47 | 66.2 | 8 | 8 | [run](https://argusic.com/run/e244f150-dc19-4354-b90f-f8ec36ca3c0c) |

## What was observed on a clean machine

Attempt 1:

- 18 min: `Qt5 not found on system - probe CMake requires Qt5`
- 6 min: `libelf and libz development headers missing (only runtime .so present)`
- 1 min: `filter_value.h and prefix_search.h missing #include <stdint.h>, bcc_per_pid_symbolizer.h missing #include <string>`
- 1 min: `tbb GCC 13 error: 'task' changes meaning of 'task'`
- 1 min: `Collector panics on k8s connectivity`
- 2 min: `Collector exits fatally when eBPF probe unavailable`
- 15 min: `Collector HTTP servers stop responding after ~60s`
- `Pre-existing test failures: prometheusexporter infinite-loop test, k8s tests with hardcoded developer paths, DNS test 'tcp_not_found' expects error_type=3 but protocol-level errors report error_type=ProtocolError (value 3, actual depends on`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
