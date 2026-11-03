# stack-diagram

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/caru-ini/stack-diagram, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/stack-diagram

## Pinned environment

- Project commit: `75dbd3e3c6fe28844322e6064d3a947b870a6c61`
- Test commit: `75dbd3e3c6fe28844322e6064d3a947b870a6c61`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4 to 4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 4 | 5 | 5 | [run](https://argusic.com/run/7c43323c-56b3-4f78-9f0d-1c520c0654ca) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System pip refused install (PEP 668 externally-managed environment)`
- 3 min: `First build failed: unresolved %%ICON_tool1%%/%%ICON_tool2%% tokens , my draft's node-section regex missed template sample nodes`
- 2 min: `'check.png' displayed image incorrect in initial test: 'file' binary not installed in container`
- 1 min: `fontTools WOFF2 probe needed brotli extension`
- 1 min: `'assets/template.html' has no token for the HTML <title> (sample '<!-- TITLE -->' leaks into output)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
