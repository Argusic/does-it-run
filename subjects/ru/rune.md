# rune

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/anomalyco/rune, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/rune

## Pinned environment

- Project commit: `565de6bb8a3449edd3dd6caa0c351bee11697964`
- Test commit: `565de6bb8a3449edd3dd6caa0c351bee11697964`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 57.2 to 61.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 32 | 61.8 | 7 | 7 | [run](https://argusic.com/run/f63950cf-5f9c-413a-9f88-01be07ebbc56) |
| 2 | fail | 20 | n/a | 57.2 | 0 | 0 | [run](https://argusic.com/run/966103a0-cabe-4bd4-b1a7-e966d32f6d42) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing libxkbcommon-dev package prevents linking without workaround`
- 5 min: `No Vulkan ICD available; GPU-dependent tests cannot run`
- 5 min: `rune lib test binary linking runs out of memory (SIGKILL) with 8GB limit`
- `rune-motion: animated_retarget_golden hash mismatch (10396150247033498793 vs expected 15969925884686696054)`
- `rune-kit markdown: an_open_span_never_shows_its_markers test fails`
- `rune alloc test: disabled_trace_hooks_neither_format_nor_allocate (201 allocations vs expected 0)`
- 3 min: `No disk space (40GB filled during builds)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
