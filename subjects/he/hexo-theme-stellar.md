# hexo-theme-stellar

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xaoxuu/hexo-theme-stellar, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/hexo-theme-stellar

## Pinned environment

- Project commit: `402e9586be07bf0c4e4d3d87f9cb9b735e630f5c`
- Test commit: `402e9586be07bf0c4e4d3d87f9cb9b735e630f5c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 7.2 | 2 | 2 | [run](https://argusic.com/run/07c3fc9d-5446-4bde-b4db-b0b1a75d226b) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `Node.js v18.19.1 below project requirement (>=22)`
- 5 min: `Integration test failed: Hexo 8.1.2 depends on strip-ansi@^7.1.0 which is ESM-only, but Hexo uses require() to load it (ERR_REQUIRE_ESM)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
