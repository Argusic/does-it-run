# fireworks-tech-graph

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yizhiyanhua-ai/fireworks-tech-graph, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/fireworks-tech-graph

## Pinned environment

- Project commit: `31fea364eda5f1852b1175f3d9e29ea31d22dcb4`
- Test commit: `31fea364eda5f1852b1175f3d9e29ea31d22dcb4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 3.4 | 2 | 2 | [run](https://argusic.com/run/8cfe9daa-32da-4bed-9cee-57b12de5101d) |

## What was observed on a clean machine

Attempt 1:

- `Node.js v18.19.1 does not satisfy puppeteer-core >=22.12.0 requirement for motion/GIF rendering`
- 5 min: `System pip3 is externally managed; cannot install Python packages system-wide without --break-system-packages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
