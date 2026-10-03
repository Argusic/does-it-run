# xiaohongshu-mcp

**Verdict: runs.** Argusic Score 90.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xpzouying/xiaohongshu-mcp, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/xiaohongshu-mcp

## Pinned environment

- Project commit: `332d196854a9eac0d2b8c2c0e3d0cc43139d724c`
- Test commit: `332d196854a9eac0d2b8c2c0e3d0cc43139d724c`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services, real run
- Valid runs: 3; wall time 12.4 to 18.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 10 | 12.4 | 0 | 0 | [run](https://argusic.com/run/2d4077d1-3a7e-4cf1-bbc5-203751df6e91) |
| 2 | pass with mocks | 92 | 13 | 17 | 1 | 1 | [run](https://argusic.com/run/dba4f8f7-e842-4425-9f36-63acc92d87f8) |
| 3 | pass | 100 | 5 | 18.3 | 2 | 2 | [run](https://argusic.com/run/70fd9d01-7117-4b68-9841-421298625544) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `Pre-compiled Chromium (148.0.7778.215) from project CDN segfaults on Ubuntu 24.04 (requires Ubuntu 22.04 or missing system libraries not installable without root)`

Attempt 3:

- 2 min: `Go (1.24.0) not installed in container`
- 18 min: `Go ulikunitz/xz library truncates large xz archives , Chromium binary extracted as 35 MB (should be 482 MB), causing segfault`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
