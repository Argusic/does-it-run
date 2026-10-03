# crosspoint-reader

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/crosspoint-reader/crosspoint-reader, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/crosspoint-reader

## Pinned environment

- Project commit: `5bfaf7bdbd847c475cad96771603b23866e83ac2`
- Test commit: `5bfaf7bdbd847c475cad96771603b23866e83ac2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.7 to 35.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 35.7 | 3 | 3 | [run](https://argusic.com/run/f66d1aac-b77f-47d3-9eec-461fb6716909) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `content_opf_parser/CMakeLists.txt used find_package(EXPAT REQUIRED) but libexpat1-dev headers not installed`
- 1 min: `chapter_html_slim_parser/CMakeLists.txt linked system expat but headers not available`
- 15 min: `PlatformIO firmware build (default env) failed: Missing toolchain directory 'None'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
