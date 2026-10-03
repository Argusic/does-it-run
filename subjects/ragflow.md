# ragflow

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/infiniflow/ragflow, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/ragflow

## Pinned environment

- Project commit: `313ca90f6abd7682fe8523e16fd67b3653a3fa84`
- Test commit: `313ca90f6abd7682fe8523e16fd67b3653a3fa84`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 39.7 to 39.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 80 | 39.7 | 7 | 7 | [run](https://argusic.com/run/10bc0432-eb19-4d88-8cab-c3208f5e1066) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing clang++ (required by build.sh)`
- 2 min: `Missing ld.lld (required to link Chromium-built pdfium)`
- 3 min: `Missing libpcre2-8.a (required by C++ tokenizer static library)`
- 2 min: `Missing cmake >= 4.0 (CMakeLists.txt requires 4.0)`
- 2 min: `Frontend build required node >= 20.19 (system had 18.19)`
- 1 min: `Frontend build OOM with default Node heap`
- `Python SDK module missing for 4 test files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
